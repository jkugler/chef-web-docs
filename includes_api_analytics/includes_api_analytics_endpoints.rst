.. The contents of this file are included in multiple topics.
.. This file should not be changed in a way that hinders its ability to appear in multiple documentation sets.


Each organization-specific authentication request must include ``/organizations/NAME`` as part of the name for the endpoint. For example, the full endpoint for editing a rule:

.. code-block:: html

   PUT /organizations/NAME/rules/ID

where ``NAME`` is the name of the organization and ``ID`` is the identifier for the rule to be edited.