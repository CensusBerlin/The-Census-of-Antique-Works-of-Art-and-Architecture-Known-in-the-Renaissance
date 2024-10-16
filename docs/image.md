**Image**

**Author:** Denitsa Nenova, George Bruseker

**Version:** 1.0


The *Image* model is intended to enable the representation and sharing of data relevant to images representing objects within the field of research.  Typical instances of the *Image* model are images representing monuments or documents that are the primary objects of scholarly discourse. *Image* is used primarily as a reference model.


| | Name| URI | 
|-|-----|-----|
|Root Ontology Node|E36 Visual Item|https://cidoc-crm.org/Entity/E36-Visual-Item/version-7.1.1 |
|Type Differentiator|N/A|N/A|



The *Image* model allows the documentation of the following kinds of information:

|Information Category | Information Collections | Description | 
|---------------------|-------------------------|-------------|
|Names and Classifications    |Names/Alternative Names/Identifiers/Type|    The researcher can document various names and classification regarding the *Image*.|
|Description  |  Description   | The researcher can document various free text descriptions of the *Image*.|

## Image **Names and Classifications**

The attribution of names and types to an *Image*, as with other entities, is a basic human activity. A chief factor in disambiguating *Images* lies in understanding the various names and identifiers that have been given to them at different moments in their individual histories. Likewise, additional classifiers of the *Image*, such as how it has been formally classified, give important distinguishing characteristics.

| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_1   | Image Identifier |   This field is used to record an identifier attributed to the documented *Image*.  |  String |   --> P1 --> E42[1_1] --> P190 --> rdfs:Literal|
|fie_2 |   Image Identifier Type  |  This field is used to record the type of the identifier attributed to the documented *Image*.  |  Concept  |  --> P1 --> E42[1_1] --> P2 --> E55[2_1]|
|fie_3  |  Image Identifier Provider |   This field is used to record the institution, group or individual responsible for providing the documented *Image*'s identifier.  |  Reference Model [Person/Group]|   --> P1 --> E42[1_1] --> P37i --> E15[3_1] --> P14 --> E39[3_2]|
|fie_5  |  Image Name |   This field is used to record the main name attributed to the documented *Image*.   | String  |  --> P1 --> E33_E41[5_1] --> P190 --> rdfs:Literal<br><br> --> P1 --> E33_E41[5_1] --> P2 --> E55[5_2]{'preferred terms'}|
|fie_10 |   Image Alias  |  This field is used to record an alternative name under which the documented *Image* is known.   | String  |  --> P1 --> E33_E41[10_1]  --> P190 --> rdfs:Literal|
|fie_11 |   Image Alias Type  |  This field is used to record the type of the alternative name that has been attributed to the documented *Image*. |   Concept |   --> P1 --> E33_E41[10_1] --> P2 --> E55[11_1]|
|fie_17  |  Image Type |   This field is used to record the formal type of the documented *Image*.  |  Concept |   --> P2 --> E55[17_1]|


### - Image Names and Classifications **Ontology Graph**
![Screenshot](img/nc_image.png)

### - Image Names and Classifications **RDF**

```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<https://census.de/example/conceptual_object/E36> a crm:E36_Visual_Item ;
    crm:P1_is_identified_by <https://example.org/name/fie_10_1>,
        <https://example.org/name/fie_1_1>,
        <https://example.org/name/fie_5_1> ;
    crm:P2_has_type <https://example.org/type/fie_17_1> .

<http://vocab.getty.edu/aat/300404670> a crm:E55_Type ;
    rdfs:label "preferred terms" .

<https://example.org/actor/fie_3_2> a crm:E39_Actor .

<https://example.org/event/fie_3_1> a crm:E15_Identifier_Assignment ;
    crm:P14_carried_out_by <https://example.org/actor/fie_3_2> .

<https://example.org/name/fie_10_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <https://example.org/type/fie_11_1> .

<https://example.org/name/fie_1_1> a crm:E42_Identifier ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <https://example.org/type/fie_2_1> ;
    crm:P37i_was_assigned_by <https://example.org/event/fie_3_1> .

<https://example.org/name/fie_5_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <http://vocab.getty.edu/aat/300404670> .

<https://example.org/type/fie_11_1> a crm:E55_Type .

<https://example.org/type/fie_17_1> a crm:E55_Type .

<https://example.org/type/fie_2_1> a crm:E55_Type .


                
```
### - Image Names and Classifications **JSON-LD**

```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "classified_as": [
        "https://example.org/type/fie_2_1"
      ],
      "content": "content",
      "id": "https://example.org/name/fie_1_1",
      "identifier_assigned_by": [
        "https://example.org/event/fie_3_1"
      ],
      "type": "Identifier"
    },
    {
      "carried_out_by": [
        "https://example.org/actor/fie_3_2"
      ],
      "id": "https://example.org/event/fie_3_1",
      "type": "IdentifierAssignment"
    },
    {
      "classified_as": [
        "http://vocab.getty.edu/aat/300404670"
      ],
      "content": "content",
      "id": "https://example.org/name/fie_5_1",
      "type": "Name"
    },
    {
      "id": "https://example.org/type/fie_2_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/fie_11_1",
      "type": "Type"
    },
    {
      "_label": "preferred terms",
      "id": "http://vocab.getty.edu/aat/300404670",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_11_1"
      ],
      "content": "content",
      "id": "https://example.org/name/fie_10_1",
      "type": "Name"
    },
    {
      "id": "https://example.org/actor/fie_3_2",
      "type": "Actor"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_17_1"
      ],
      "id": "https://census.de/example/conceptual_object/E36",
      "identified_by": [
        "https://example.org/name/fie_10_1",
        "https://example.org/name/fie_5_1",
        "https://example.org/name/fie_1_1"
      ],
      "type": "VisualItem"
    },
    {
      "id": "https://example.org/type/fie_17_1",
      "type": "Type"
    }
  ]
}
                
```

## Image **Description**

*Images* are the subjects of innumerable descriptions that provide a wide range of information with regards to the aesthetic and historical importance of the work, inter alia. Such descriptions are of use in a scholarly understanding of an *Image* only if we are able to track the provenance of such elocutions in a systematic fashion. Such an aim drives the need for the tracking of description information as a separate category. The descriptor necessary to this task are documented in the table below.

| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_188    |Image Description  |  This field is used to record a description in free text of the documented *Image*.  |  String  ||  --> P129i --> E33[188_1] --> P190 --> rdfs:Literal

### - Image Description **Ontology Graph**
![Screenshot](img/desc_image.png)

### - Image Description **RDF**

```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .

<https://census.de/example/conceptual_object/E36> a crm:E36_Visual_Item ;
    crm:P129i_is_subject_of <https://example.org/conceptual_object/fie_188_1> .

<https://example.org/conceptual_object/fie_188_1> a crm:E33_Linguistic_Object ;
    crm:P190_has_symbolic_content "content" .


```

### - Image Description **JSON-LD**

```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "content": "content",
      "id": "https://example.org/conceptual_object/fie_188_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://census.de/example/conceptual_object/E36",
      "subject_of": [
        "https://example.org/conceptual_object/fie_188_1"
      ],
      "type": "VisualItem"
    }
  ]
}
                
```
