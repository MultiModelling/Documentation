Creating a use-case
===================

To have a new use-case, you need to prepare a DAG file and a configuration file.

DAG file
--------
.. note::

    This section will not explain how to create a DAG file from scratch.
    You can review already created examples in `Multi Modelling Model Repository <https://github.com/MultiModelling/Model-Repository>`_.
    `Apache Airflow Documentation <https://airflow.apache.org/docs/apache-airflow/2.6.3/core-concepts/dags.html>`_ provides more generic information on DAGs.

Airflow DAGs are defined in Python language. These are regular ``.py`` files and they have to be placed under a folder in the ``dags`` directory in `Model-Orchestrator <https://github.com/MultiModelling/Model-Orchestrator>`_.
These DAGs must contain the definitions of the **task**s that will run consecutively.
A task can be created with the ``Operator`` classes of Airflow.

Example use-cases use ``PythonOperator``s for most of their tasks, which they are generic for this project.
These operators are ``subroutine_initialize``, ``subroutine_computation`` and ``subroutine_finalize``.

A task that uses ``subroutine_initialize`` operator has to be created. In the examples, it is named as ``Initialize``.
For ``subroutine_finalize`` operator, the task in the examples is ``Finalize``.
For each step that is going to require an interaction with a **Model Adapter**, we need a separate task that utilises ``subroutine_computation``.

This is an example task called ``My_model``, which utilises ``subroutine_computation``:

.. code-block:: python

    My_model = PythonOperator(dag=dag,
                            task_id='My_model',
                            python_callable=subroutine_computation)

Note that there is no information on configuration and how to use the model. These are going to be provided with a configuration file and will be referenced with the name of the task.
In this case, this is ``My_model``.

Finally, tasks order can be defined with ``>>`` operator. The task on the right side of the operator will run after the one on the left side.
Example:

.. code-block:: python

    Initialize >> My_model >> Finalize

This will trigger ``Initialize`` first, then ``My_model``, and finally ``Finalize``.

Repeating tasks
^^^^^^^^^^^^^^^

If a task, or group of multiple tasks needs to be repeated in the DAG, a function that returns the running order of *one repetition* can be created as follows:

.. code-block:: python

    def group(number, **kwargs):
        dyn_value = "{{ task_instance.xcom_pull(task_ids='push_func') }}"

        with TaskGroup(group_id=f'Iteration_{number}') as tg1:
            t1 = PythonOperator(dag=dag,
                        task_id=f'First_repeated_task_{number}',
                        python_callable=subroutine_computation)

            t2 = PythonOperator(dag=dag,
                        task_id=f'Second_repeated_task_{number}',
                        python_callable=subroutine_computation)

            t1 >> t2

        return tg1

Then repetition can be achieved as in the following example:

.. code-block:: python

    prev = Initialize >> Task_A
    iters = 2
    for i in range(1,iters+1):
        item = group(i)
        if prev is not None:
            prev >> item
        prev = item
    prev >> Task_B >> Finalize

The running order will be: ``Initialize``, ``Task_A``, ``First_repeated_task_1``, ``Second_repeated_task_1``, ``First_repeated_task_2`` ``Second_repeated_task_2``, ``Task_B``, ``Finalize``.


Configuration file
------------------

This file includes configuration information about a specific run of a use-case.
It is written in JSON format. It consists of 4 sections:

1. ``metadata`` section includes information to identify a task. These are: experiment, project, run, scenario and user. The directory going to be used in Minio for input/output files is selected according to the values under the metadata.
2. ``modules`` includes the address of the Model Registry.
3. ``databases`` holds a dictionary of connection parameters for each of the databases going to be used by models.
4. ``tasks`` holds a dictionary of the configuration of each task in the DAG that this configuration is going to be used with. Key of the dictionary item has to be mach with task name in the DAG. Contents of the ``model_config`` key is specific to the model that is going to be used.

Example configuration:

.. code-block:: json

    {
        "metadata": {
            "experiment": "Trial_1",
            "project": "tholen",
            "run": "MM_workflow_run_1",
            "scenario": "v05-26kw",
            "user": "mmvib"
        },
        "modules": {
            "model_registry": "http://mmvib-registry:9200/registry/"
        },
        "databases": {
            "Influx": {
                "api_addr": "influxdb:8086",
                "db_config": {
                    "db_name": "energy_profiles",
                    "use_ssl": false
                }
            },
            "Minio": {
                "api_addr": "minio:9000",
                "db_config": {
                    "access_key": "admin",
                    "secret_key": "password",
                    "secure": false
                }
            }
        },
        "tasks": {
            "Task_A": {
                "api_id": "Model_A",
                "model_config": {
                    "input_esdl_file_path": "test/input.esdl",
                    "output_esdl_file_path": "test/1/output.esdl"
                },
                "type": "computation"
            },
            "Task_B": {
                "api_id": "Model_B",
                "model_config": {
                    "action": "some_action",
                    "action_config": {
                        "some_action": {
                            "input_esdl_file_path": "test/1/output.esdl",
                            "output_esdl_file_path": "test/2/output.esdl"
                        }
                    },
                    "some_config": {
                        "some_val": "sample"
                    }
                },
                "type": "computation"
            }
        }
    }
