Prerequisites
=============

This software stack is designed to run on docker, using docker-compose on Linux.
The minimum versions required are listed in the table below.

=============== ========
Software        Versions
=============== ========
Docker Engine   20.10.22
Docker Compose  2.14.1
Python          3.11
Apache Airflow  2.6.3
=============== ========

It is known to be working on Ubuntu 22.10 and RHEL 8.7.

For the installation of Docker Engine and Compose, you can follow: https://docs.docker.com/engine/install/

Development with Python 3.11
----------------------------

Components of MMviB run in containers. These containers are configured to use Python 3.11.
You do not need to install Python on your system if you are going to run all components with Docker Compose.

If you need to run components that require Python on your bare metal host for development purposes, you need to use Python 3.11.
Older versions *might* work, but it is not guaranteed.

To install Python 3.11 on Ubuntu systems that does not have 3.11 on main repository (22.04 and older):

.. code-block:: console

    sudo add-apt-repository ppa:deadsnakes/ppa
    sudo apt-get update
    sudo apt install python3.11

Using a different `venv <https://docs.python.org/3.11/library/venv.html>`_ for each components is recommended.