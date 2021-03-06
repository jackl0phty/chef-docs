.. The contents of this file are included in multiple topics.
.. This file describes a command or a sub-command for Knife.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.


The ``show`` argument is used to display information about the specified environment. 

This argument has the following syntax::

   knife environment show ENVIRONMENT_NAME

This argument does not have any argument-specific options.

**Examples**

For example, to view information about the "dev" environment enter:

.. code-block:: bash

   $ knife environment show dev
   
to return:

.. code-block:: bash

   % knife environment show dev
   chef_type:            environment
   cookbook_versions:
   default_attributes:
   description:
   json_class:           Chef::Environment
   name:                 dev
   override_attributes:
    
   \\
   \\ 
   \\
   \\

To view information in |json| format, use the ``-F`` common option as part of the command like this:

.. code-block:: bash

   $ knife environment show dev -F json

Other formats available include ``text``, ``yaml``, and ``pp``.
