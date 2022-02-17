
========
Mongodb
========

Mongo database

Install mongodb container:

.. code-block:: powershell

    D:\Teguh\docker>docker pull mongo

Running mongodb container:

.. code-block:: powershell

    D:\Teguh\docker>docker run -it -d -p 27017:27017 -v mongodata:/data/db --name mongodb mongo

------------------