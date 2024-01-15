Installing Minio
================

Clone the repo and change directory to cloned repo:

.. code-block:: console

    git clone https://github.com/MultiModelling/Database-MinIO.git
    cd Database-MinIO

Create a ``.env`` file for overriding default username and password:

.. code-block:: bash

    MINIO_ROOT_USER=admin
    MINIO_ROOT_PASSWORD=password

Run Minio in the background with the following command:

.. code-block:: console

    docker compose up -d

Now it shoud be accessible on ``http://localhost:9090``.
You can access Minio using credentials defined in ``.env`` file.

Now you can create a bucket called ``test`` by following the information on the next section.

-------
Buckets
-------

Later on, you can create, view or delete buckets via **Buckets** page, which can be accessed via left side of the Minio's dashboard, or ``http://localhost:9090/buckets``.
Buckets are used by your DAGs and adapters to store input/output files used/created by models in a pipeline.

Inside of a bucket is organised like a folder.
You can alter contents of a bucket via **Object Browser** (on menu), or ``http://localhost:9090/browser``.