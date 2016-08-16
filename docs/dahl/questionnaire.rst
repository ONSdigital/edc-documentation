Questionnaire Object
====================

The Questionnaire object contains the top level questionnaire attributes and is
defined below:

.. code-block:: JavaScript
  :linenos:

  {
      "mime_type": "application/json/ons/eq",
      "questionnaire_id": "0",
      "schema_version": "0.0.1",
      "survey_id": "0",
      "title": "Star Wars",
      "theme": "starwars",
      "description": "Kitchen sink test for the Star Wars questionnaire",
      "introduction": {
          "description": "May the force be with you"
      },
      "display": {
          "properties": {}
      },
      "eq_id": "0",
      "messages": {
        "INTEGER_TOO_LARGE": "Too big, that number is",
        "NEGATIVE_INTEGER": "It must be a positive number",
        "NOT_INTEGER": "Please enter an integer"
      },
      "groups": [...]
  }

.. glossary::

    Line 2: defines the mime-type for the questionnaire.  This is a constant and should not be changed
    Line 3: is the form type
    Line 4: is the version number for this schema
    Line 5: is the numeric id of the Survey that this questionnaire is a part of
    Line 6: is the title of the questionnaire
    Line 7: declares which theme/look-and-feel is used when the questionnaire is presented to the respondent
    Line 8: is the description of the questionnaire displayed in the author application
    Line 9: defines the questionnaire introduction as an object.  Currently only one property is declared which is the introductory text on line 10.  Later versions may also allow the legal notice to be customised.
    Line 12: defines some properties to influence the display of the questionnaire (not yet implemented)
    Line 15: is the Unique eQ id of the questionnaire.  Unlike survey_id and questionnaire_id, this is unique across all questionnaires
    Line 16: The message object allows questionnaire-level overriding of built-in error messages
    Line 21: The array of groups within the questionnaire
