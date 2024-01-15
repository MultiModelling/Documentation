Installing Model Registry
=========================

Clone the repo and change directory to cloned repo:

.. code-block:: console

    git clone https://github.com/MultiModelling/Model-Registry.git
    cd Model-Registry

To use ``memorydb`` implemented within the registry instead of an external Postgre instance,
you should edit the option ``DB_TYPE`` to ``memorydb`` in ``.env.docker`` file.
Alternatively, you can set up a PostgreSQL instance and edit the ``.env.docker`` accordingly.

After preparing your ``.env.docker`` file, you can use the following command to run Model Res=gistry in background:

.. code-block:: console

    docker compose up -d

To list registered model adapters, you can use:

.. code-block:: console

    curl localhost:9200/registry/ | jq '.[]'

Initially this will return nothing, as newly launched registry will be empty. You can try running this again after you deploy new adapters in following sections.