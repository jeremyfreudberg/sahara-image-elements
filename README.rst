Sahara image elements project
==============================

This is the massopencloud branch of sahara-image-elements project. Here is where it differs from upstream version:

* Installs Pig  
* Sets all environment variables for Hadoop/Hive/Pig/Java in both "hadoop" and "ubuntu" users 
* Installs Midori 

Note that to submit a Pig job in YARN (at least when done via Sahara EDP) you need to set `yarn.resourcemanager.scheduler.class` to `org.apache.hadoop.yarn.server.resourcemanager.scheduler.fair.FairScheduler`. This can be done by specifying in Sahara node-group template, or manually. 

.. sourcecode:: bash

    tox -e venv -- sahara-image-create -p vanilla -i ubuntu
