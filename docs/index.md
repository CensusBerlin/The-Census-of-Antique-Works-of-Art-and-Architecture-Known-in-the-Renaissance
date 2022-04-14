# Introduction
 
The [Census Semantic Data Models](http://census.de/csdm) (CSDM) represent a coherent set of semantically-encoded data models for the use of art historians in the (re-)representation of art historical data related to the history of monuments, the documents that respond to or bear witness to them, the people or places that relate to these objects of study through historical events, and the images and bibliography which reference them. 
 
The CSDM has been built from three major sources:
 
## 1) The Census Data Model
 
The immediate scope and representational direction of the CSDM has been guided by the original data and data model of [The Census of Antique Works of Art and Architecture Known in the Renaissance](https://www.census.de) (Institut für Kunst- und Bildgeschichte, Humboldt-Universität zu Berlin). The Census project - which began in 1946, developed over decades as a system of index cards and photographs, and was first computerised in the early 1980s - provides a time-tested foundation from which to build a set of semantic data models of use to art historical research. The Census was created in the 1940s with the goal of replacing what was then a vague notion of “classical influence” in the Renaissance with a specific knowledge of which antique monuments were known in the Renaissance, in which setting, and in which condition. Over its more than seventy-five-year history the Census has traced Renaissance artists’ and humanists’ response to antiquities, and has had at its core the documentation of events which connect artists and authors with particular antique monuments. The Census dataset has become a tool useful for archaeologists who are interested, for example, the condition and state of preservation of antiquities in the Renaissance and for historians and art historians concerned with the creative reception of antiquities during the Renaissance period. 
 
It is a core objective of the CSDM to provide a new representation of the Census data that enables its faithful re-representation in a semantic format, allowing for researchers to query it according to a common logic.
 
 
 
## 2) The CIDOC CRM
 
The [CIDOC CRM (CIDOC Conceptual Reference Model)](http://cidoc-crm.org) offers itself as an appropriate framework, as a formal ontology which allows for the representation of Cultural Heritage data in general in a common form. The CRM is an event-based model whose form enables the rich representation and connection of data from heterogeneous data models into a common system. The passage to Linked Open Data is richest when this data is represented in a common format that is well documented and openly accessible to a wider community of scholars. The CRM enables precisely this transition. The event-centred modelling strategy of the ontology, furthermore, is highly compatible with the existing abstract data model of the Census, making the choice of this ontology the most appropriate.
 
## 3) The SARI Reference Data Models
 
While the CRM provides a general language and framework for the semantic representation of cultural heritage data, it explicitly refrains from specifying how it should be implemented in any particular context, leaving the standard open to adoption and evolution according to new needs and requirements. At the same time, the CRM enables the creation of a common set of well-understood methods for representing data that can be read and adopted both by end users of the data (researchers) and by those who create and support the systems which allow access to the data (developers).
 
[SARI (Swiss Art Research Infrastructure, Universität Zürich)](https://www.sari.uzh.ch/) is an infrastructure which has adopted the CIDOC CRM in order to enable widely-interoperable cultural heritage (CH) data about art history, *inter alia*. To support this strategy, using the CIDOC CRM they have invested in and developed the [SRDM (Semantic Reference Data Models)](https://docs.swissartresearch.net/), a set of well-documented, fundamental semantic modelling patterns suited to research on the visual arts. They have created the SRDM to represent basic targets of cultural heritage documentation and to provide well-documented patterns that can be adopted in representing entities as well as the typical information collected in relation to them. The CSDM thus takes up the CIDOC CRM though the SRDM modelling, adopting its basic patterns and representation in order to follow existing best practice and to join and add to a growing community of like-minded users wishing to share semantic data.
 
The immediate use of CSDM documentation is to act as an explicit documentation and specification of the semantic data structures used to represent the Census data as Linked Open Data. Users of this documentation can refer to this paper as a guide to the overall semantic modelling decisions that were taken during this project, as well as a detailed description of each model that was created and the information that it enables the researcher to encode or query. 
 
The broader purpose of this documentation is both to empower researchers to query the existing Census data that has been represented semantically and to enable the possibility of integrating this data by using and/or extending the CSDM. The Census data is offered in a semantic format as LOD in order to open Census data to a broader uptake by scholars and, moreover, to expand the data in unforeseen ways that extend beyond the scope of corpus-building projects such as the Census. 
 
 
# Methodology
Reuse of SRDM, create a subset, any additions documented with their own notation in a compatible format.
# Contents of CSDM
The CSDM is, then, a series of semantic data models, which follows the SRDM patterns and enables the documentation of key objects (monuments, documents) and supporting data regarding people, places and bibliography. It enables a rich representation and querying of this data by its use of the CIDOC CRM, which joins the models through a robust documentation of events connecting the various entities.
 
The Corpus of CSDM includes:
 
 
|Name | Description | CRM Entity | SARI Equivalent |
|-----|-------------|------------|-----------------|
|Monument|  This model is intended to enable the representation and sharing of data relevant to artistic, architectural and historical artefacts extant in the past or present. In the Census, *Monuments* are antique inscriptions, coins, paintings, sculptures, architectural monuments and other ancient artefacts and works of art. In some cases, *Monuments* can also be works of art and architecture which are not antique, but were believed in the Renaissance to be antique.|   E22 Human Made Object   | Builtwork
|Document|  This model is intended to enable the representation and sharing of data relevant to physical items, which carry content that provides evidence of a historical witnessing of, response to or reference to a particular *Monument*. In the Census, this category can include drawings, prints, paintings, medals, and statuettes, or written documents such as printed guidebooks, manuscripts, letters and inventories.   | E22 Human Made Object  |  Archival Item |
|Person| This model is intended to enable the representation and sharing of data relevant to real-world, physical persons. |  E21 Person   | Person|
|Location| This model is intended to enable the representation and sharing of data relevant to geographic places used to identify the locations of items and events over time.  |  E53 Place |   Place|
|Bibliography| This model is intended to enable the representation and sharing of data relevant to bibliographic sources that have been used in the course of researching and documenting.| E33 Linguistic Object  |  Bibliographic Entity |
|Image|  This model is intended to enable the representation and sharing of data relevant to images representing objects within the field of research.  |  E36 Visual Item    | Image |
|Period| This model is intended to enable the documentation and correct referencing of historical periods for use in datation.  |  E4 Period    | N/A |
 
Each of these models supports a separate unit of documentation adopted in the Census. An instance of such a model stands for one real-world entity that is documented by that instance. The models exist in relation, joining on key relations in order to create a web of supporting interrelations that represent the real-world historical trajectory of objects through time and space, and map specific instances of the reception of antique monuments by post-classical observers. While event-centric modelling is used, the events are recorded within the context of the objects to which they relate (e.g.: birth relative to the individual, production relative to the monument/document). For the purpose of documentation, this allows separate objects to be documented in separate models. Within the context of an open graph network of facts, the event nodes can be used to traverse a complex historical graph of observations of and responses to antique objects through time.
 


