Useful tips
===========

Apache-Airflow
--------------

On a Windows OS, run Apache-Airflow from a Ubuntu(Linux)-WSL terminal. Running from a PowerShell terminal will show errors. You can check 
the activeness of WSL by typing the terminal command ``wsl --version``. 

Minio
-----
#. Docker run command for starting a `minio container <https://min.io/docs/minio/container/index.html>`_:

.. code-block:: python
    docker run \
        -p 9000:9000 \
        -p 9001:9001 \
        --name minio1 \
        -v D:\minio\data:/data \
        -e "MINIO_ROOT_USER=<ROOTUSER>" \
        -e "MINIO_ROOT_PASSWORD=<CHANGEME123>" \
        quay.io/minio/minio server /data --console-address ":9001"

Environment variables such as ``v`` can be adjusted according to the location of your working folder/directory. 

#. (continue...)

Docker
------

#. The command ``docker compose up -d --no-deps --build airflow-webserver airflow-scheduler`` is used for executing building and running 
docker-compose.yaml file after making changes to it.

#. The command ``curl -Lf0 'https://airflow.apache.org/docs/apache-airflow/<version_number>/docker-compose.yaml'`` is used to download 
docker-compose.yaml file in the current directory. The current ``<version_number>`` is 2.9.2 (dated 17th June 2024). 

#. The command ``docker compose down -v --remove-orphans`` is used to remove a stopped containers, along with removing its volumes. 

#. For working within a container, the command ``docker exec -it <container_id> <command>`` is used, where ``i`` is the interactive mode 
(keep STDIN open even if not attached). An example of `<command>` is *sh*, which creates a new shell. 

After working with the container, it can be restarted with the command ``docker start -ai <container_id>``. 

#. To get into the main process id within the container, use the command ``docker inspect -f {{'.State.Pid'}} <container_id>``. 

