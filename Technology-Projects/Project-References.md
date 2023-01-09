

Goal:  
Make it easier to have references in markdown.
Have a global list of references; with metadata to help in finding/sorting/discovery
Ability to include references into a markdown document, based on a keyword (JSON) pre-processor concept.   

Existing Challenges:
markdown syntax is []() - difficult to type.

Idea:
A JSON database, with all references.
Some basic input form to write to the database.
Ability to view/read/sort/search DB

Writing : get a unique-id in UI that can be used in editing process to include reference in the document/markdown.
Validating : validate DB for link-rot...

# Future Expansion
- References to podcasts, etc.


# Technology:
## DB
DB - mongodb / ? / couchbase /
DB - simple non
DB - couchbase - capella - fully managed cloud service eliminates your database fully managed cloud service eliminates your database

## Serializing (I thought this was old-stype...)
Python serializer
- marshmallow - https://marshmallow.readthedocs.io/
- MIT pydantics - https://pydantic-docs.helpmanual.io/benchmarks/
- ??
