Installing Adapters
===================

Here, installation steps for adapters used in MMviB listed.
Instructions for the first adapter (TEACOS) are given in more detail.
Since instructions are similar, installation instructions for the following adapters will only include brief descriptins followed by commands and configs.

TEACOS
------

Clone the repo and change directory to cloned repo:

.. code-block:: console

    git clone https://github.com/MultiModelling/teacos-adapter.git
    cd teacos-adapter

Edit ``.env.docker`` file to add Minio username and password you used while installing Minio.
Alternatively, you can create an access key for this adapter and use it.

.. code-block:: bash

    #username
    MINIO_ACCESS_KEY=fill_in
    #password
    MINIO_SECRET_KEY=fill_in

To let your adapter establish a connection to TEACOS, you should provide following values in ``.env.docker`` file.

.. code-block:: bash

    TEACOS_API_URL=fill_in
    TEACOS_USER=fill_in
    TEACOS_ENV=fill_in
    TEACOS_PASSWORD=fill_in

And following values are for the database instance going to be accessed by TEACOS.

.. code-block:: bash

    DATABASE_HOST=fill_in
    DATABASE_NAME=fill_in
    DATABASE_USER=fill_in
    DATABASE_PASSWORD=fill_in

Finally, execute the following for running the adapter at the bachround:

.. code-block:: console

    docker-compose up -d

To check if the adapter is registered in the Model registry, use the following command:

.. code-block:: console

    curl localhost:9200/registry/ | jq '.[]'

ESSIM
-----

Clone:

.. code-block:: console

    git clone https://github.com/MultiModelling/Adapter-ESSIM.git
    cd Adapter-ESSIM

Edit ``.env.docker``:

.. code-block:: bash

    MINIO_ACCESS_KEY=admin
    MINIO_SECRET_KEY=password

Run:

.. code-block:: console

    docker-compose up -d

ETM-KPIs
--------

Clone:

.. code-block:: console

    git clone https://github.com/MultiModelling/Adapter-ETM-KPIs.git
    cd Adapter-ETM-KPIs

Edit ``.env.docker``:

.. code-block:: bash

    MINIO_ACCESS_KEY=admin
    MINIO_SECRET_KEY=password

Run:

.. code-block:: console

    docker-compose up -d

Adapter-ConnectInfra
--------------------

Clone:

.. code-block:: console

    git clone https://github.com/MultiModelling/Adapter-ConnectInfra.git
    cd Adapter-ConnectInfra

Edit ``.env.docker``:

.. code-block:: bash

    MINIO_ACCESS_KEY=admin
    MINIO_SECRET_KEY=password

Run:

.. code-block:: console

    docker-compose up -d

Adapter-Regionalization
-----------------------

Clone:

.. code-block:: console

    git clone https://github.com/MultiModelling/Adapter-Regionalization.git
    cd Adapter-Regionalization

Edit ``.env.docker``:

.. code-block:: bash

    MINIO_ACCESS_KEY=admin
    MINIO_SECRET_KEY=password

Run:

.. code-block:: console

    docker-compose up -d

Opera
-----

This adapter require Windows to run.

MOTER
-----

This adapter require Windows to run.