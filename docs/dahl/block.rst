Block Object
============

The block object is one of the workhorses of the eq platform.  It primarily acts
as a navigable unit in that each block is displayed as a page within eq.

Each block has an id which is what is displayed with the url of the survey runner
and the users route through the questionnaire is defined as moving from block to
block.

A block has a number of sections and validation rules, although block-level
validation has not yet been implemented.  The sections contain questions, while
routing rules direct the user from block to block.

.. code-block:: JavaScript
   :linenos:

   {
       "display": {
           "properties": {}
       },
       "id": "f22b1ba4-d15f-48b8-a1f3-db62b6f34cc0",
       "sections": [...],
       "routing_rules":[...],
       "title": "",
       "validation": []
   }
