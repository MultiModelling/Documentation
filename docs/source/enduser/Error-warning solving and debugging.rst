Error-Warning solving and debugging
===================================

Apache Airflow
--------------

If accessing via the localhost ``http://localhost:8080`` is not happening as you might be redirected to ``http://localhost:8080/auth``, you can 
forcefully try to change to ``http://localhost:8080/login``. If this also does not work try clearing cache on your web-browser. This issue happens 
if some other application have used this port in the past, for example, keycloak (used by the ESSIM model). 


Port issues
-----------

If you try to connect to a port used by some other application, you will get an error message regarding this on your terminal. Then, you can check this 
by the command ``net-stat -ano | findstr <port_number>`` (in a command prompt or power shell). An example of ``port_number`` can be ``8080``. 

You can then kill the existing application/activity, if not needed elsewhere, using the command ``taskkill /PID <PID> /F``. Sometimes, you might get a 
``permission-denied`` error when using the above command. If so, change to adminstrative mode in powershell, for example. 


Python errors
-------------

When running the files manually, you might get the error: 'tno' module not found. To avoid this error, enter the following lines before the 
``from tno.---`` line in the Python script: 

.. code-block:: Python

    import sys
    sys.path.append("../<folder_name>")

``<folder_name>`` represents the folder within which the ``tno`` folder is located. 


Minio errors
------------

1. Sometimes, you might encounter an error related to maximum connection timeout related to connecting to Minio server. For localhost, this means that a 
Minio instance need to be activated from an independent terminal. 

2. You might see an error related to S3 operation failed. This could mean that the bucket is not present (or created), path to finding the bucket is not 
correct, the path to find an object within the bucket is not found, or a combination of these. This can be rectified by creating the bucket (whose name 
might be found in the config .json file, model.py file, or <name_of_the_model>.py file) or correcting the path (check for variables named 
<input/output>_esdl_file_path, base_path, destination_path, etc.).

3. Sometimes, you might encounter a connection error (for example, access keys not correct, or something similar). In this case, check if there is a 
difference between the Minio instance and .env file in terms of ``MINIO_ACCESS_KEY`` / ``ROOT_USER_NAME`` or ``MINIO_SECRET_KEY`` / 
``ROOT_USER_PASSWORD``. 
