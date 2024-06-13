Steps to reproduce cases in your own personal environment
=========================================================

Step 1 # Setting up Docker
--------------------------

Install docker desktop. Depending upon your Operating System (OS), steps might be different. 
The following link provides the installation steps of different OS

.. code-block:: console

    https://docs.docker.com/engine/install/ 


You may not have to install Docker if you do not wish to run the code in a containerized environment. 
This might happen if you want to run separate components of model adapters or other components of the IT infrastructure separately.
To be on the safe side, I would still suggest to install Docker Desktop. 

Step 2 # Setting up Orchestrator
---------------------------------

* General set up *

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

* Project-specific set up *

In this project, it is instructed to use Airflow in a Docker environment. See instructions steps in :ref:`Installing Apache Airflow`. 


If you get UID warning on your OS and want to avoid this, you can created an environment or ``.env`` file (if not created) and 
write ``AIRFLOW_UID=50000``. Non-linux systems might give errors when running the command 
``AIRFLOW_UID=$(id -u) docker compose up -d``. If that's the case, you can simply run ``docker compose up`` command. ``-d`` is 
for running in detached mode, inputting which is not neccessary. In addition, you also do not need to set up ``USERNAME`` and ``PASSWORD`` 
in the ``.env`` file as they have been taken care of in the ``docker compose`` file under the services ``airflow-init``. Environment file
command just overrides the set up in the Docker Compose file, as mentioned in the instructions.  

If accessing via the localhost ``http://localhost:8080`` is not happening, you can try ``http://localhost:8080/login``. If still you 
cannot access the web-browser, the reason might be that the port ``8080`` is used by some other application. If this is the case, you 
will get an error message on your terminal. You can check this by the following command (in a command prompt or power shell):

.. code-block:: console

    net-stat -ano | findstr :8080


You can then kill the existing application/activity, if not needed elsewhere, using the following 
command:
.. code-block:: console

    taskkill /PID <PID> /F

This will forcefully kill the PID corresponding to the port ``8080``.




you can check the container ``model-orchestrator`` within the container tab in the Docker Desktop. Within 
the container, you can look at the service ``



# After login, you will see a screen with example DAGs created for MMviB.
# To be able to successfully trigger them, Minio and Model Adapters are required.