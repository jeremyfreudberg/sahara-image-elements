Sahara image elements project
==============================

This is the massopencloud branch of sahara-image-elements project. Here is where it differs from upstream version:

* Installs Pig  
* Sets all environment variables for Hadoop/Hive/Pig/Java in both "hadoop" and "ubuntu" users  
* Allows YARN to handle Pig jobs submitted by Sahara -- by changing scheduler type to "Fair Scheduler" (**this feature coming soon**)  

.. sourcecode:: bash

    tox -e venv -- sahara-image-create -p vanilla -i ubuntu
