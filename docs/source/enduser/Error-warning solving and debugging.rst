Error Debug
===========

Apache Airflow
--------------

If accessing via the localhost ``http://localhost:8080`` is not happening as you might be redirected to ``http://localhost:8080/auth``, you can 
forcefully try to change to ``http://localhost:8080/login``. If this also does not work try clearing cache on your web-browser. This issue happens 
if some other application have used this port in the past, for example, keycloak (used by the ESSIM model). 


Port issues
-----------

If you try to connect to a port used by some other application, you will get an error message regarding this on your terminal. Then, you can check this 
by the command ``net-stat -ano | findstr <port_number>`` (in a command prompt or power shell). An example of ``port_number`` can be ``8080``. 

You can then kill the existing application/activity, if not needed elsewhere, using the command `taskkill /PID <PID> /F`. Sometimes, you might get a 
``permission-denied`` error when using the above command. If so, change to adminstrative mode in powershell, for example. 
