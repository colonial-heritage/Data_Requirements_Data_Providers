## Minimal requirements data providers | Datahub (CONCEPT)

### Location, date, material, subjects, type, maker, object data provider
| Topic/Field | Data Requirement |
|----------|----------|
| Where do we search in?   | all text fields and thesauri labsels max 250 characters.  |
| Location information    | Present as much as possible, modeled as Geonams or TGN  |
| If no alignment possible    | Geonames   |
| Which location is relevant?    | Location of creation  |
| Location name    | present day name of location and as precise as possible through identifier   |
| location requirements    | universal  |
| Date    | XSD, Integer on year level. Through CIDOC CRM it can be a range   |
| Material    | NMVW thesaurus or one that is aligned. AAT and CHT also used often. Alignment could be made by us*  |
| Facets and labels    | English - AAT and Dutch CHT ?  |
| Foreign parties*  | May need AAT?  |
| Subjects*   | NMVW thesaurus, follows the above  |
| Type   | NMVW thesaurus, follows the above  |
| Maker   | link to constituents in RA and map Wikidata/RKDartists to our constituents. Communities to be added to constituentsgraph  |
| Object data provider   | register in dataset register of NDE or ours, responsibility on data provider  |


## Object
| Topic/Field | Data Requirement |
|----------|----------|
|Images|NDE requirements: IIIF|
|Open text fields|to be determined which. max 250 words|

### Provenance
| Topic/Field | Data Requirement |
|----------|----------|
|Model Architect Datahub| [repo](https://github.com/colonial-heritage/data-models?tab=readme-ov-file) and [model](https://github.com/colonial-heritage/data-models/blob/main/provenance-events/conceptual.md) with Linked Art|
|Design UX/UI Designer Datahub|[UX/UI Design Research App](https://gui-prototype.colonialcollections.nl/object.html)|
|Linked art|as interpreted by Sjors*|
|All entities|PID required|
|Type|aquisition vs transfer of custodyin CIDOC CRM; what is the claim here?|
|Classification|for nuance previous point, AAT|
|Qualifiers|Further nuance through Probably or Possibly, if NONE than sure, if less than Possibly dont deliver Provenance. AAT|
| Name | String, no max length|
| Description | same |
| Source | dont require citation |
| Transferred from and to | constituents, to be added to graph |
| Location | Geonames, rethink NMVW |
| Date | Integers, structured, XSD |
| Start after and Ends before | ID of other provenance event/record, Link to events on time line, has to be provenance record, scope = provenance of the same object |
| Related to | Events of Wikidata |

### Constituents - Person RDF Model
| Topic/Field | Data Requirement |
|----------|----------|
|identification| minimal information to identify person |
| Dublicates | Same as relationship |
| Date | Integer  |
| Location | Geonames |
| Description | String, no max length | 
| Source | dont require citation | 

Ideally now difference between Person and Organization, only in Type.

### Organisation
| Topic/Field | Data Requirement |
|----------|----------|
| Date of foundation | Integer XSD |
| Date of determination | Integer XSD |
| Location | Geonames |
| Duplicates | Same as relationship |

### Images
| Topic/Field | Data Requirement |
|----------|----------|
|Images|IIIF, Image and Publication API|

### Data description
| Topic/Field | Data Requirement |
|----------|----------|
|  after NDE standards
