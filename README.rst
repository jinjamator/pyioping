Introduction
==================

Pyioping is an abstraction layer to simplify programatic use of the ioping binary for linux. It was written to have a simple interface for test setups. 


Features
-----------------

Pyioping has following features:
    * create and manage ioping instances
    * get results of instances by parsing output to python datastructures.
    * register callbacks intermediate results.

Installation
------------

Install pyioping by running:

.. code-block:: bash

    pip3 install pyioping


Examples
---------

Create a unicast udp 1000pps setup and test for 10 seconds
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: python

    test2 = IOPingInstance()
    test2.set_options(name=1,test_path="/tmp",interval=0.1)
    test2.start()
    test = IOPingInstance()
    test.set_options(name=2,test_path="/srv",interval=0.1)
    test.start()


Supported Parameters
---------------------

To see all supported parameters for the set_options function, review the constructor of the IOPingInstance object.


Contribute
----------

- Issue Tracker: https://github.com/jinjamator/pyioping/issues
- Source Code: https://github.com/jinjamator/pyioping

Roadmap
-----------------

Selected Roadmap items:
    * add class documentation

For documentation please refer to https://pyioping.readthedocs.io/en/latest/

License
-----------------

This project is licensed under the Apache License Version 2.0