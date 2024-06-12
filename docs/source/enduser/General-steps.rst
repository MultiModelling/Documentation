Steps to reproduce cases in your own personal environment
=========================================================

Step 1
------

Install docker desktop. Depending upon your Operating System (OS), steps might be different. 
The following link provides the installation steps of different OS

.. code-block:: console

    https://docs.docker.com/engine/install/ 


You may not have to install Docker if you do not wish to run the code in a containerized environment. 
This might happen if you want to run separate components of model adapters or other components of the IT infrastructure separately.
To be on the safe side, I would still suggest to install Docker Desktop. 

Step 2
-------
You may or may not have to install the Orchestrator (Apache Airflow, in our case) in your own OS environment. 
To not have to install Airflow, you must install Docker Desktop. 
Apache Airflow provide a 'Docker Compose' file which can be downloaded from their official website and can be run
as a following command in a terminal:

.. code-block:: console

    docker compose up

The detailed instruction, including the Docker Compose file, for airflow installation and run in a Docker environment can be found in 
the following link:

.. code-block:: bash

    https://airflow.apache.org/docs/apache-airflow/2.9.2/howto/docker-compose/index.html

General installation instructions can be following in the following link:

.. code-block:: console

    https://airflow.apache.org/docs/apache-airflow/2.9.2/installation/index.html

It is not advisable to install airflow directly on Windows OS. It is handled properly by 
having Linux Subsystem, such as WSL, installed in such a system. 

In this project, it is instructed to use Airflow in a Docker environment. See instructions steps in :ref:`Installing Apache Airflow` 

.. code-block:: console

    https://multimodelling.readthedocs.io/en/latest/installation/Installing%20Apache%20Airflow.html

If you get UID warning on your OS and want to avoid this, you can created an ``.env`` file (if not created) and 
write ``AIRFLOW_UID=50000``. Non-linux systems might give errors when running the command 
``AIRFLOW_UID=$(id -u) docker compose up -d``. 




Create a ``.env`` file for overriding default username and password with following contents:

.. code-block:: bash

    _AIRFLOW_WWW_USER_USERNAME=airflow
    _AIRFLOW_WWW_USER_PASSWORD=airflow

Run Airflow in the background with the following command:

.. code-block:: console

    AIRFLOW_UID=$(id -u) docker compose up -d

Now it should be accessible on ``http://localhost:8080``.
You can access it using credentials defined in ``.env`` file.

After login, you will see a screen with example DAGs created for MMviB.
To be able to successfully trigger them, Minio and Model Adapters are required.