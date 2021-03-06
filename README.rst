**************
DEVOPS Menu
**************



A menu system for DEVOPS.
===========================

Why
------------
I got tired of running all kinds of scripts to manage things.


Requirements
==============

- pyyaml
- six
- jinja2
- boto3


Example
============

.. code-block:: bash

    +------------------------------------------------------------------------------
    Main Menu
    +------------------------------------------------------------------------------
    [1] | All/General/Other
    +------+-----------------------------------------------------------------------
    [0] | Quit
    +------------------------------------------------------------------------------



Installation
=============
`pip install devops-menu`. This will install the scripts in /usr/share/devops-menu folder.

Note: Install manually with 'sudo -H python setup.py install' if not installing with pip.

Note:  Make sure your ~/.aws config and credentials files are setup correctly with the profile
to the various AWS instances.


Example config:
=================

.. code-block:: bash

    [default]
    output = json
    region = us-east-1

    [profile test1]
    output = json
    region = us-east-1

    [profile test2]
    output = json
    region = us-east-1



Example credentials:
======================

.. code-block:: bash

    [default]
    aws_access_key_id = xxx
    aws_secret_access_key = xxx

    [test1]
    aws_access_key_id = xxx
    aws_secret_access_key = xxx

    [test2]
    aws_access_key_id = xx
    aws_secret_access_key = xxx



For script usage, run the following command:

.. code-block:: bash

    devops-menu


Configuration
===============
If you want to add more scripts or modify the menu, got to /usr/share/devops-menu and edit the devops-menu.yml file and
add the scripts to the scripts directory.

It is best to follow the same yml format in the menu file, and the same format in the bash scripts.



Updates
==========
- 10/31/18 Initial commit

Copyright
===========

Copyright 2015 Will Rubel

Based on easy-menu python module by mogproject.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
