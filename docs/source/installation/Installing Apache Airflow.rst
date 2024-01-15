Installing Apache Airflow
=========================

Clone the repo and change directory to cloned repo:

.. code-block:: console

    git clone https://github.com/MultiModelling/Model-Orchestrator.git
    cd Model-Orchestrator

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