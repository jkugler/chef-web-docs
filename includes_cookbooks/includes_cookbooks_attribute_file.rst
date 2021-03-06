.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.

An attribute file is located in the ``attributes/`` sub-directory for a cookbook. When a cookbook is run against a node, the attributes contained in all attribute files are evaluated in the context of the node object. Node methods (when present) are used to set attribute values on a node. For example, the ``apache2`` cookbook contains an attribute file called ``default.rb``, which contains the following attributes:

.. code-block:: ruby

   default['apache']['dir']          = '/etc/apache2'
   default['apache']['listen_ports'] = [ '80','443' ]

The use of the node object (``node``) is implicit in the previous example; the following example defines the node object itself as part of the attribute:

.. code-block:: ruby

   node.default['apache']['dir']          = '/etc/apache2'
   node.default['apache']['listen_ports'] = [ '80','443' ]
