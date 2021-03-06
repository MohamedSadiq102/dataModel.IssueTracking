# Civic Issue Tracking data models

These data models allow to perform civic issue tracking. They have been designed
with a view to enabling trivial interoperability between FIWARE NGSI version 2 and
NGSI-LD and [Open311](http://www.open311.org/). As a result, property names have not
been normalized to the `camelCase`syntax, they remain as currently specified by
Open311. That is the rationale behind naming entity types with `Open311` as
prefix. However, a few properties are added, so that FIWARE NGSI version 2
implementations can properly store and serve Open 311 data.

In the medium term, might propose to the Open311 Community a harmonized data model
aligned with the rest of smart data models and schema.org. In fact, using these
data models and a FIWARE NGSI version 2 o rNGSI-LD implementation it is trivial
to implement the APIs proposed by Open311. Another option would be the use of
[JSON-LD](http://json-ld.org) to define equivalencies and mappings between a
FIWARE / Schema.org data model and Open 311.

The FIWARE NGSI civic issue tracking data model defines the following entity
types:

-   [`Open311:ServiceType`](https://swagger.lab.fiware.org/?url=https://smart-data-models.github.io/dataModel.IssueTracking/Open311_ServiceType/swagger.yaml). A type of service
    a citizen can request. It encompasses data from the Open 311 GET Service
    List and GET Service Definition.
-   [`Open311:ServiceRequest`](https://swagger.lab.fiware.org/?url=https://smart-data-models.github.io/dataModel.IssueTracking/Open311_ServiceRequest/swagger.yaml). A specific
    service request (of a service type) made by a citizen.
