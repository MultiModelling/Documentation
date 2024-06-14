Steps to reproduce cases in your own personal environment
=========================================================


Step 1 # Setting up Docker
--------------------------

Install docker desktop. Depending upon your Operating System (OS), steps might be different. 
The `Install Docker Engine <https://docs.docker.com/engine/install/>`_ website provides the installation steps in different OS.

You may not have to install Docker if you do not wish to run the code in a containerized environment. 
This might happen if you want to run separate components of model adapters or other components of the IT infrastructure separately.
To be on the safe side, I would still suggest to install Docker (Docker Desktop is for Windows). 


Step 2 # Setting up Orchestrator
---------------------------------

* General set-up

You may or may not have to install the Orchestrator (Apache Airflow, in our case) in your own OS environment. 
To not have to install Airflow, you must install Docker Desktop. 
Apache Airflow provide a 'Docker Compose' file which can be downloaded from their official website and can be run
as a command ``docker compose up`` in a terminal.

The detailed instruction, including the Docker Compose file, for airflow installation and run in a Docker environment can be found in 
the `Running Airflow in Docker <https://airflow.apache.org/docs/apache-airflow/2.9.2/howto/docker-compose/index.html>`_ website.
  

General installation instructions can be following in the `Installation of Airflow <https://airflow.apache.org/docs/apache-airflow/2.9.2/installation/index.html>`_
website.

It is not advisable to install airflow directly on Windows OS. It is handled properly by 
having Linux Subsystem, such as WSL, installed in such a system. 

* Project-specific set-up 

In this project, it is instructed to use Airflow in a Docker environment. See instruction steps in :ref:`Installing Apache Airflow`. 
A general suggestion is to create a virtual environment in the new directory after cloning from GitHub. This avoids conflicts between 
global and local python packages, along with other advantages one can find on the internet. See instructions for creating `virtual 
environment <https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/>`_ in differnt environments.

If you get UID warning on your OS and want to avoid this, you can created an environment or ``.env`` file (if not created) and 
write ``AIRFLOW_UID=50000``. Non-linux systems might give errors when running the command 
``AIRFLOW_UID=$(id -u) docker compose up -d``. If that's the case, you can simply run ``docker compose up`` command. ``-d`` is 
for running in detached mode, inputting which is not neccessary. In addition, you also do not need to set up ``USERNAME`` and ``PASSWORD`` 
in the ``.env`` file as they have been taken care of in the ``docker compose`` file under the services ``airflow-init``. Environment file
command just overrides the set up in the Docker Compose file, as mentioned in the instructions.  



Step 3 # Minio installation and connection
------------------------------------------

* General set-up

`Installing Minio <https://min.io/docs/minio/windows/index.html>`_ provides instructions for installing and deploying Minio in your personal environment. 
This webpage takes you to the Windows OS, but has tabs for other environments such as Kubernetes, Docker, Linux, and macOS. 

This generally accesses the port ``9000``. You can use ``http://localhost:9000`` or ``http://127.0.0.1:9000`` on your web-browser. 

* Project-specific set-up

For this docker need to be installed and running on your system. See instruction steps in :ref:`Installing Minio`. You can adjust the volumes within 
Minio services of the ``docker compose`` file to redirect to a specific file location/directory for your Minio activity, such as creating buckets, 
editing, and removing them. A folder can be created within the directory ``Database-MinIO``, and location can be included in the volumes. 



Step 4 # Model registry installation
--------------------------------------

This keeps track of all model adapter services that are active on your environment. Follow the instruction steps in :ref:`Installing Model Registry`. 



Step 5 # Installation of model adapters
---------------------------------------

Either you can install all model adapters or case-specific model adapters from GitHub (see :ref:`Installing Adapters`).


Step 6 # Running a case
-----------------------

:ref:`Running a use-case` provides basic information to familiarize with the Orchestrator, Apache-Airflow, interface. If step 2 is performed correctly, 
you could see DAGs on your locahost screen. :ref:`Creating a use-case` acquints you with tasks, operators, etc. used in this project for different cases. 

We focused on a sample case of ``etm_essim_demo``. For this, the following model adapters need to be running on your Docker environment: 
1. ESSIM
2. ETM-Price-Profile
3. ESDL-Add-Price-Profile

Apart from these, the following repository components need to also run on Docker:
1. Database-MinIO
2. Model-Registry
3. Model-Orchestrator

(continue...)
