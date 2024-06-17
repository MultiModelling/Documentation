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
  

General installation instructions can be following in the 
`Installation of Airflow <https://airflow.apache.org/docs/apache-airflow/2.9.2/installation/index.html>`_ website.

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

If step 2 is performed correctly, you could see DAGs on your locahost screen. :ref:`Creating a use-case` acquints you with tasks, 
operators, etc. used in this project for different cases. 

We focused on a sample case of ``etm_essim_demo``. For this, the following model adapters need to be running on your Docker environment: 

#. ESSIM

#. ETM-Price-Profile

#. ESDL-Add-Price-Profile


Apart from these, the following repository components need to also run on Docker:

#. Database-MinIO

#. Model-Registry

#. Model-Orchestrator


:ref:`Running a use-case` provides basic information to familiarize with the Orchestrator, Apache-Airflow, interface. For the ``etm_essim_demo`` 
DAG, the **Trigger DAG w/ config** shows a blank configuration JSON object. This needs to filled with etm_essim_demo.json data (copy-paste the 
entire content). The current JSON file (present in the model repository) is giving errors. This was rectified and 
`here <https://github.com/MultiModelling/Documentation/blob/main/docs/source/enduser/etm_essim_demo.json>`_. 

.. literalinclude:: ./etm_essim_demo.json
   :language: json
   :linenos:
   :caption: Object description


(Optional) Alternative Step # Manual running or checking of adapters (without using Docker)
----------------------------------------------------------------------------------

Once you have cloned all the above-mentioned adapters and other repository components mentioned in Step 6, you can run the ``main:app`` of each of them. 
This python file is found within the folder ``tno\<application_name>``. For example, for the ESSIM adapter, the application name is ``essim_adapter``. 
To run the file from the base directory, you can use the command ``python tno\<application_name>\main.py``. N.B.: ``\`` or ``/`` depends on your OS. 

To avoid encountering any issues, first start the model registry. Then, model adapters can be started. Each adapter will register itself to the registry. 
You can check this on the webbrowser with ``http://localhost:9900/registry``. ``9900`` port is exposed for manual run (see the ``.env`` file of each 
adapter). 

For the manual set up, a local minio instance need to run on your OS or local environment (see 'General set-up' in Step 3) from a separate or dedicated 
terminal. 

 

