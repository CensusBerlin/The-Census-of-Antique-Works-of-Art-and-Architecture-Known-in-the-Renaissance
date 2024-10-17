**Antique Monument**

**Author:** Denitsa Nenova, George Bruseker

**Version:** 1.0

The *Antique Monument* model is intended to enable the representation and sharing of data relevant to artistic and architectural artefacts extant in the past or present. An instance of the *Antique Monument* model is typically a work of art or architecture created in antiquity which is the subject of art historical research. In the context of the Census, this research is especially concerned with the changing nature of knowledge about this object, or the reception of this object by artists and other observers during the Renaissance. The Census is concerned with questions of whether particular antique *Antique Monuments* were extant in and known in the Renaissance, which artists and observers knew them, where these *Antique Monuments* were, and their condition over time. It is also concerned with the impact of *Antique Monuments* upon the creation of new works of art and literature in the period 1400-1600. Part of this investigation includes research into how ancient *Antique Monuments* were collected, studied, or restored, or whether they were simply ‘known’ and were therefore part of the visual culture of the time. 

Instances of the *Antique Monument* model may also include deliberate falsifications of antiquities, or objects which were judged incorrectly in the Renaissance period to be antique. 




| | Name| URI | 
|-|-----|-----|
|Root Ontology Node|E22 Human-Made Object | https://cidoc-crm.org/Entity/E22-Human-Made-Object/version-7.1.1|
|Type Differentiator |monuments | http://vocab.getty.edu/aat/300006958 |

The *Antique Monument* model allows the documentation of the following kinds of information:

|Information Category | Information Collections | Description | 
|---------------------|-------------------------|-------------|
|Names and Classifications    |Names/Alternative Names/Identifiers/Type/Style/Cause of Observation|   The researcher can document various names and classification regarding the *Antique Monument*.|
|Existence    |Production/Destruction|  The researcher can document the events related to the production and destruction of a *Antique Monument*. |
|Events    |Modification/Provenance Event|    The researcher can document events leading to changes to the *Antique Monument* over time and changes in its provenance history.|
|Locations   | Location |   The researcher can document the location of the *Antique Monument*.|
|Designation Status |   Condition  |  The researcher can document the condition state of a *Antique Monument* over time.|
|Description  |  Description   | The researcher can document various free text descriptions of the *Antique Monument*.|
|Documentation  | Citation/Image/External URI| The researcher can document citations relative to the *Antique Monument*, link to images of the *Antique Monument* and document external URIs of documentation for the same *Antique Monument*.|

## Antique Monument **Names and Classifications**

The attribution of names and types to *Antique Monument*, as with other entities, is a basic human activity. A chief factor in disambiguating *Antique Monuments* lies in understanding the various names and identifiers that have been given to them at different moments in their individual histories. Likewise, additional classifiers of the *Antique Monument*, such as how it has been classified as an object as such, give important distinguishing characteristics.


| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_5  |  Monument Name  |  This field is used to record the main name attributed to the documented *Antique Monument*.  |  String  |  --> P1 --> E33_E41[5_1] --> P190 --> rdfs:Literal<br><br> --> P1 --> E33_E41[5_1] --> P2 --> E55[5_2]{'preferred terms'}|
|fie_10  |  Monument Alias  |  This field is used to record an alternative name under which the documented *Antique Monument* is known.  |  String  |  --> P1 --> E33_E41[10_1]  --> P190 --> rdfs:Literal|
|fie_11  |  Monument Alias Type  |  This field is used to record the type of the alternative name that has been attributed to the documented *Antique Monument*.  |  Concept |   --> P1 --> E33_E41[10_1] --> P2 --> E55[11_1]|
|fie_16  |  Monument Alias Source |   This field is used to record the source on the basis of which the organization attributing the alternative name use based their attribution.  |  Reference Model [Bibliographic Entity/Image] |  --> P1 --> E33_E41[10_1] --> P141i --> E13[15_1] --> P16 --> E73[16_1]|
|fie_1  |  Monument Identifier  |  This field is used to record an identifier attributed to the documented *Antique Monument*.  |  String |   --> P1 --> E42[1_1] --> P190 --> rdfs:Literal|
|fie_2  |  Monument Identifier Type |   This field is used to record the type of the identifier attributed to the documented *Antique Monument*.  |  Concept |   --> P1 --> E42[1_1] --> P2 --> E55[2_1]|
|fie_3  |  Monument Identifier Used By |   This field is used to record the institution, group or individual responsible for providing the documented *Antique Monument*'s identifier. |   Reference Model [Person/Group]|   --> P1 --> E42[1_1] --> P37i --> E15[3_1] --> P14 --> E39[3_2]|
|fie_17 |   Monument Type  |  This field is used to record the formal type of the documented *Antique Monument*.   | Concept |   --> P2 --> E55[17_1]|
|fie_cen_83 |   Monument Type Uncertainty  |  This field is used to record the concept of uncertainty defining the formal type of the documented *Antique Monument*. |   Collection [Uncertainty] |  --> P2 --> E55[17_1] --> P141i --> E13[C83_1]|
|fie_cen_21 |   Monument Class |   This field is used to record a metatype of the documented *Antique Monument*.  |  Concept  |  --> P2 --> E55[C21_1] --> P2 --> E55[C21_2]|
|fie_cen_81 |   Monument Class Uncertainty |   This field is used to record the concept of uncertainty defining the classification of the documented *Antique Monument*.    |Collection  [Uncertainty]|  --> P2 --> E55[C21_1] --> P2 --> E55[C21_2] --> P141i --> E13[C81_1]|
|fie_201  |  Monument Style  |  This field is used to record the style by which the documented *Antique Monument* can be classified with or for which it is exemplary.  |  Concept |   --> P2 --> E55[201_1]<br><br> --> P2 --> E55[201_1] --> P2 --> E55 "Style"[201_2]|
|fie_cen_84 |   Monument Style Uncertainty  |  This field is used to record the concept of uncertainty defining the formal style of the documented *Antique Monument*.    |Collection [Uncertainty]|   --> P2 --> E55[201_1] --> P2 --> E55[201_2] --> P141i --> E13[C84_1]|
|fie_cen_56 |   Monument Cause of Observation  |  This field is used to record the cause of observation of the documented *Antique Monument*. |    Concept |   --> P2 --> E55[C56_1] --> P2 --> E55[C56_2]|
|fie_cen_80  |  Monument Cause of Observation Uncertainty  |  This field is used to record the concept of uncertainty defining the cause of observation of the documented *Antique Monument*. |   Collection  [Uncertainty]|  --> P2 --> E55[C56_1] --> P2 --> E55[C56_2] --> P141i --> E13[C80_1]|

### - Antique Monument Names and Classifications **Ontology Graph**
![Screenshot](img/nc_monument.png)

### - Antique Monument Names and Classifications **RDF**

```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P1_is_identified_by <https://example.org/name/fie_10_1>,
        <https://example.org/name/fie_1_1>,
        <https://example.org/name/fie_5_1> ;
    crm:P2_has_type <https://example.org/type/C21_1>,
        <https://example.org/type/C56_1>,
        <https://example.org/type/fie_17_1>,
        <https://example.org/type/fie_201_1> .

<http://vocab.getty.edu/aat/300404670> a crm:E55_Type ;
    rdfs:label "preferred terms" .

<https://example.org/actor/fie_3_2> a crm:E39_Actor .

<https://example.org/conceptual_object/fie_16_1> a crm:E73_Information_Object .

<https://example.org/event/C80_1> a crm:E13_Attribute_Assignment .

<https://example.org/event/C81_1> a crm:E13_Attribute_Assignment .

<https://example.org/event/C83_1> a crm:E13_Attribute_Assignment .

<https://example.org/event/C84_1> a crm:E13_Attribute_Assignment .

<https://example.org/event/fie_15_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/fie_16_1> .

<https://example.org/event/fie_3_1> a crm:E15_Identifier_Assignment ;
    crm:P14_carried_out_by <https://example.org/actor/fie_3_2> .

<https://example.org/name/fie_10_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P141i_was_assigned_by <https://example.org/event/fie_15_1> ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <https://example.org/type/fie_11_1> .

<https://example.org/name/fie_1_1> a crm:E42_Identifier ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <https://example.org/type/fie_2_1> ;
    crm:P37i_was_assigned_by <https://example.org/event/fie_3_1> .

<https://example.org/name/fie_5_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <http://vocab.getty.edu/aat/300404670> .

<https://example.org/type/C21_1> a crm:E55_Type ;
    crm:P2_has_type <https://example.org/type/C21_2> .

<https://example.org/type/C21_2> a crm:E55_Type ;
    crm:P141i_was_assigned_by <https://example.org/event/C81_1> .

<https://example.org/type/C56_1> a crm:E55_Type ;
    crm:P2_has_type <https://example.org/type/C56_2> .

<https://example.org/type/C56_2> a crm:E55_Type ;
    crm:P141i_was_assigned_by <https://example.org/event/C80_1> .

<https://example.org/type/fie_11_1> a crm:E55_Type .

<https://example.org/type/fie_17_1> a crm:E55_Type ;
    crm:P141i_was_assigned_by <https://example.org/event/C83_1> .

<https://example.org/type/fie_201_1> a crm:E55_Type ;
    crm:P2_has_type <https://example.org/type/fie_201_2> .

<https://example.org/type/fie_201_2> a crm:E55_Type ;
    rdfs:label "Style" ;
    crm:P141i_was_assigned_by <https://example.org/event/C84_1> .

<https://example.org/type/fie_2_1> a crm:E55_Type .


                
```

### - Antique Monument Names and Classifications **JOSN-LD**     
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "classified_as": [
        "https://example.org/type/fie_17_1",
        "https://example.org/type/C21_1",
        "https://example.org/type/fie_201_1",
        "https://example.org/type/C56_1"
      ],
      "id": "https://census.de/example/physical_object/E22",
      "identified_by": [
        "https://example.org/name/fie_10_1",
        "https://example.org/name/fie_5_1",
        "https://example.org/name/fie_1_1"
      ],
      "type": "HumanMadeObject"
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
      "id": "https://example.org/type/fie_11_1",
      "type": "Type"
    },
    {
      "assigned_by": [
        "https://example.org/event/fie_15_1"
      ],
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
      "carried_out_by": [
        "https://example.org/actor/fie_3_2"
      ],
      "id": "https://example.org/event/fie_3_1",
      "type": "IdentifierAssignment"
    },
    {
      "id": "https://example.org/event/C81_1",
      "type": "AttributeAssignment"
    },
    {
      "id": "https://example.org/event/C83_1",
      "type": "AttributeAssignment"
    },
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
      "id": "https://example.org/event/C84_1",
      "type": "AttributeAssignment"
    },
    {
      "id": "https://example.org/event/C80_1",
      "type": "AttributeAssignment"
    },
    {
      "assigned_by": [
        "https://example.org/event/C81_1"
      ],
      "id": "https://example.org/type/C21_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/conceptual_object/fie_16_1",
      "type": "InformationObject"
    },
    {
      "_label": "Style",
      "assigned_by": [
        "https://example.org/event/C84_1"
      ],
      "id": "https://example.org/type/fie_201_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/fie_2_1",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_201_2"
      ],
      "id": "https://example.org/type/fie_201_1",
      "type": "Type"
    },
    {
      "_label": "preferred terms",
      "id": "http://vocab.getty.edu/aat/300404670",
      "type": "Type"
    },
    {
      "assigned_by": [
        "https://example.org/event/C80_1"
      ],
      "id": "https://example.org/type/C56_2",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/type/C21_2"
      ],
      "id": "https://example.org/type/C21_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/event/fie_15_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/fie_16_1"
      ]
    },
    {
      "classified_as": [
        "https://example.org/type/C56_2"
      ],
      "id": "https://example.org/type/C56_1",
      "type": "Type"
    },
    {
      "assigned_by": [
        "https://example.org/event/C83_1"
      ],
      "id": "https://example.org/type/fie_17_1",
      "type": "Type"
    }
  ]
}
                
```                           

## Antique Monument **Existence**

Of essential import in identifying and tracking *Antique Monuments* is information pertaining to their existence in time, particularly information regarding the creation and destruction of the monument. For this reason, we have clustered descriptors relevant to such information in a common ‘existence’ category. These are described in the table below.

| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_299  |  Monument Creation Type |   This field is used to indicate the type of production activity used in the production of the documented *Antique Monument*.  |  Concept  |  --> P108i --> E12[58_1] --> P2 --> E55[299_1]|
|fie_cen_96 |   Monument Creator |   This field is used to record the actor who has created the documented *Antique Monument*. |   Reference Model [Person/Group]|   --> P108i --> E12[58_1] --> P01i --> PC14[C96_1] --> P02 --> E39[C96_2]|
|fie_cen_97  |  Monument Creator Role |   This field is used to record the specific role of the actor they played in the creation of the documented *Antique Monument*.  |  Concept |   --> P108i --> E12[58_1] --> P01 --> PC14[C96_1] --> P14.1 --> E55[C97_1]|
|fie_cen_42  |  Monument Creator Attribution  |  This field is used to record the attribution type (renaissance or contemporary) assigning the creator of the documented *Antique Monument*.  |  Concept  |  --> P108i --> E12[58_1]  --> P01i --> PC14[C96_1] --> P02 --> E39[C96_2] --> P141i --> E13[C42_1] --> P2 --> E55[C42_2]|
|fie_cen_43 |   Monument Creator Source |   This field is used to relate a document carrying a textual reference about the attribution (Renaissance or contemporary) assigning the creator of the documented *Antique Monument* and the documented *Antique Monument* itself. |    Reference Model [Document]|   --> P108i --> E12[58_1]  --> P01--> PC14[C96_1] --> P02 --> E39[C96_2] --> P141i --> E13[C42_1] -- >P16 --> E33[C43_1] --> P128i --> E22[C43_2]|
|fie_58  |  Monument Creation Earliest Date  |  This field is used to record the earliest possible date for the production of the documented *Antique Monument*.|    Date |   --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P82a --> xsd:dateTime|
|fie_59 |   Monument Creation Latest Date |   This field is used to record the latest possible date for the production of the documented *Antique Monument*.  |  Date |   --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P82b --> xsd:dateTime|
|fie_61 |   Monument Creation Falls Within  |  This field is used to record the historical period in which the production of the documented *Antique Monument* occurred.   | Reference Model  [Period]|  --> P108i --> E12[58_1] --> P10 --> E4[61_1]|
|fie_cen_44 |   Monument Creation Date Attribution  |  This field is used to record the attribution type (Renaissance or contemporary) assigning the timespan of the production of the documented *Antique Monument*.  |  Concept  |  --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P141i --> E13[C44_1] --> P2 --> E55[C44_2]|
|fie_cen_45  |  Monument Creation Date Source  |  This field is used to relate a document carrying a textual reference about the attribution (renaissance or contemporary) assigning a timespan of the production of the documented *Antique Monument* and the documented *Antique Monument* itself.   | Reference Model [Document]|   --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P141i --> E13[C44_1] --> P16 --> E33[C45_1] --> P128i --> E22[C45_2]|
|fie_60 |   Monument Creation Location  |  This field is used to record the place of the production of the documented *Antique Monument*. |   Reference Model [Location]|   --> P108i --> E12[58_1] --> P7 --> E53[60_1]|
|fie_cen_46  |  Monument Creation Location Attribution |   This field is used to record the attribution type (Renaissance or contemporary) assigning the place of production of the documented *Antique Monument*.  |  Concept  |  --> P108i --> E12[58_1] --> P7 --> E53[60_1] --> P141i --> E13[C46_1] --> P2 --> E55[C46_2]|
|fie_cen_47 |   Monument Creation Location Source  |  This field is used to relate a document carrying a textual reference about the attribution (Renaissance or contemporary) assigning the place of production of the documented *Antique Monument* and the documented *Antique Monument* itself. |   Reference Model  [Document]|  --> P108i --> E12[58_1] --> P7 --> E53[60_1] --> P141i --> E13[C46_1] --> P16 --> E33[C47_1] --> P128i --> E22[C47_2]|
|fie_cen_8  |  Monument Destruction Type |   This field is used to record the formal type of the destruction event of the documented *Antique Monument*.   |  Concept |   --> P13i --> E6_E7[62_1] --> P2 --> E55[C8_1]|
|fie_cen_9 |   Monument Destruction Actors Involved |   This field is used to record the actor carried out he destruction event of the documented *Antique Monument*.   |  Reference Model   [Person/Group]| --> P13i --> E6_E7[62_1] --> P01i --> PC14[C16_1] --> P02 --> E39[C9_1]|
|fie_cen_16 |   Monument Destruction Actor Role |   This field is used to record the specific capacity in which the actor carried out the destruction event of the documented *Antique Monument*. |   Concept |   --> P13i --> E6_E7[62_1] --> P01 --> PC14[C16_1] --> P14.1 --> E55[C16_2]|
|fie_cen_17 |   Monument Destruction Actor Attribution  |  This field is used to record the attribution type (Renaissance or contemporary) assigning the actor carried out he destruction event of the documented *Antique Monument*. |    Concept  |  --> P13i --> E6_E7[62_1] --> P01i --> PC14[C16_1] --> P02 --> E39[C9_1] -- P141i --> E13[C17_1] --> P2 --> E55[C17_2]|
|fie_cen_18 |   Monument Destruction Actor Source  |  This field is used to relate a document carrying a textual reference about the attribution (Renaissance or contemporary) assigning the actor carried out he destruction event  of the documented *Antique Monument* and the documented *Antique Monument* itself.   | Reference Model [Document]|   --> P13i --> E6_E7[62_1] --> P01i --> PC14[C16_1] --> P02 --> E39[C9_1] -- P141i --> E13[C17_1] -- >P16 --> E33[C18_1] --> P128i --> E22[C18_2]|
|fie_cen_7 |   Monument Destruction Date |   This field is used to record the general timespan of the destruction event of the documented *Antique Monument*.    |Collection [Timespan]|   --> P13i --> E6_E7[62_1]  --> P4 --> E52[62_2]|
|fie_cen_99 |   Monument Destruction Period |   This field is used to record the period during which the destruction event of the documented *Antique Monument* has happened.   | Reference Model [Period]|   --> P13i --> E6_E7[62_1] --> P10 --> E4 [C99_1]|
|fie_cen_102 |   Monument Destruction Location  |  This field is used to record the destruction location of the documented *Antique Monument*.  |  Reference Model [Location]|   --> P13i --> E6_E7[62_1]  --> P7 --> E53[102_1]|
|fie_cen_103  |  Monument Destruction Location Attribution  |  This field is used to record the attribution type (Renaissance or contemporary) assigning the destruction location of the documented *Antique Monument*. |   Concept |   --> P13i --> E6_E7[62_1] --> P7 --> E53[102_1]--> P141i -->E13[C103_1] --> P2 --> E55[C103_2]|
|fie_cen_104 |   Monument Destruction Location Attribution Source  |  This field is used to relate a document carrying a textual reference about the attribution (Renaissance or contemporary) assigning the destruction location of the documented *Antique Monument*.  |  Reference Model  [Document]|  --> P13i --> E6_E7[62_1] --> P7 --> E53[102_1] --> P141i -->E13[C103_1]  --> P16 -->E33[C104_1] --> P128i --> E22[C104_2]|

### - Antique Monument Existence **Ontology Graph**
![Screenshot](img/ex_monument.png)

### - Antique Monument Existence **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P108i_was_produced_by <https://example.org/event/fie_58_1> ;
    crm:P13i_was_destroyed_by <https://example.org/event/fie_62_1> .

<https://example.org/actor/C96_2> a crm:E39_Actor ;
    crm:P141i_was_assigned_by <https://example.org/event/C42_1> .

<https://example.org/actor/C9_1> a crm:E39_Actor ;
    crm:P141i_was_assigned_by <https://example.org/event/C17_1> .

<https://example.org/conceptual_object/C18_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C18_2> .

<https://example.org/conceptual_object/C43_1> a crm:E33_Linguistic_Object ;
    crm:P128i_carried_by <https://example.org/physical_object/C43_2> .

<https://example.org/conceptual_object/C45_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C45_2> .

<https://example.org/conceptual_object/C47_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C47_2> .

<https://example.org/event/C17_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C18_1> ;
    crm:P2_has_type <https://example.org/type/C17_2> .

<https://example.org/event/C42_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C43_1> ;
    crm:P2_has_type <https://example.org/type/C42_2> .

<https://example.org/event/C44_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C45_1> ;
    crm:P2_has_type <https://example.org/type/C44_2> .

<https://example.org/event/C46_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C47_1> ;
    crm:P2_has_type <https://example.org/type/C46_2> .

<https://example.org/event/fie_58_1> a crm:E12_Production ;
    crm:P01i_is_domain_of <https://example.org/property/C96_1> ;
    crm:P10_falls_within <https://example.org/event/fie_61_1> ;
    crm:P2_has_type <https://example.org/physical_object/fie_299_1> ;
    crm:P4_has_time-span <https://example.org/time_span/fie_58_2> ;
    crm:P7_took_place_at <https://example.org/place/fie_60_1> .

<https://example.org/event/fie_61_1> a crm:E4_Period .

<https://example.org/event/fie_62_1> a crm:E6_Destruction,
        crm:E7_Activity ;
    crm:P01i_is_domain_of <https://example.org/property/C16_1> ;
    crm:P2_has_type <https://example.org/type/C8_1> ;
    crm:P4_has_time-span <https://example.org/time_span/fie_62_2> .

<https://example.org/physical_object/C18_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C43_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C45_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C47_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/fie_299_1> a crm:E55_Type .

<https://example.org/place/fie_60_1> a crm:E53_Place ;
    crm:P141i_was_assigned_by <https://example.org/event/C46_1> .

<https://example.org/property/C16_1> a crm:PC14_carried_out_by ;
    crm:P02_has_range <https://example.org/actor/C9_1> ;
    crm:P14.1_in_the_role_of <https://example.org/type/C16_2> .

<https://example.org/property/C96_1> a crm:PC14_carried_out_by ;
    crm:P02_has_range <https://example.org/actor/C96_2> ;
    crm:P14.1_in_the_role_of <https://example.org/type/C97_1> .

<https://example.org/time_span/fie_58_2> a crm:E52_Time-Span ;
    crm:P141i_was_assigned_by <https://example.org/event/C44_1> ;
    crm:P82a_begin_of_the_begin ""^^xsd:dateTime ;
    crm:P82b_end_of_the_end ""^^xsd:dateTime .

<https://example.org/time_span/fie_62_2> a crm:E52_Time-Span .

<https://example.org/type/C16_2> a crm:E55_Type .

<https://example.org/type/C17_2> a crm:E55_Type .

<https://example.org/type/C42_2> a crm:E55_Type .

<https://example.org/type/C44_2> a crm:E55_Type .

<https://example.org/type/C46_2> a crm:E55_Type .

<https://example.org/type/C8_1> a crm:E55_Type .

<https://example.org/type/C97_1> a crm:E55_Type .

```

                
### - Antique Monument Existence **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/physical_object/fie_299_1",
      "type": "Type"
    },
    {
      "crm:P02_has_range": {
        "id": "https://example.org/actor/C9_1"
      },
      "crm:P14.1_in_the_role_of": {
        "id": "https://example.org/type/C16_2"
      },
      "id": "https://example.org/property/C16_1",
      "type": "crm:PC14_carried_out_by"
    },
    {
      "id": "https://example.org/physical_object/C45_2",
      "type": "HumanMadeObject"
    },
    {
      "destroyed_by": "https://example.org/event/fie_62_1",
      "id": "https://census.de/example/physical_object/E22",
      "produced_by": "https://example.org/event/fie_58_1",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/type/C8_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/physical_object/C43_2",
      "type": "HumanMadeObject"
    },
    {
      "carried_by": [
        "https://example.org/physical_object/C47_2"
      ],
      "id": "https://example.org/conceptual_object/C47_1",
      "type": "LinguisticObject"
    },
    {
      "classified_as": [
        "https://example.org/type/C42_2"
      ],
      "id": "https://example.org/event/C42_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C43_1"
      ]
    },
    {
      "crm:P128i_carried_by": {
        "id": "https://example.org/physical_object/C43_2"
      },
      "id": "https://example.org/conceptual_object/C43_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/C44_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/C42_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/C46_2",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/physical_object/fie_299_1"
      ],
      "crm:P01i_is_domain_of": {
        "id": "https://example.org/property/C96_1"
      },
      "falls_within": [
        "https://example.org/event/fie_61_1"
      ],
      "id": "https://example.org/event/fie_58_1",
      "timespan": "https://example.org/time_span/fie_58_2",
      "took_place_at": [
        "https://example.org/place/fie_60_1"
      ],
      "type": "Production"
    },
    {
      "id": "https://example.org/event/fie_61_1",
      "type": "Period"
    },
    {
      "assigned_by": [
        "https://example.org/event/C17_1"
      ],
      "id": "https://example.org/actor/C9_1",
      "type": "Actor"
    },
    {
      "carried_by": [
        "https://example.org/physical_object/C18_2"
      ],
      "id": "https://example.org/conceptual_object/C18_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/C17_2",
      "type": "Type"
    },
    {
      "crm:P02_has_range": {
        "id": "https://example.org/actor/C96_2"
      },
      "crm:P14.1_in_the_role_of": {
        "id": "https://example.org/type/C97_1"
      },
      "id": "https://example.org/property/C96_1",
      "type": "crm:PC14_carried_out_by"
    },
    {
      "id": "https://example.org/physical_object/C18_2",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/type/C16_2",
      "type": "Type"
    },
    {
      "assigned_by": [
        "https://example.org/event/C42_1"
      ],
      "id": "https://example.org/actor/C96_2",
      "type": "Actor"
    },
    {
      "id": "https://example.org/physical_object/C47_2",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/type/C97_1",
      "type": "Type"
    },
    {
      "carried_by": [
        "https://example.org/physical_object/C45_2"
      ],
      "id": "https://example.org/conceptual_object/C45_1",
      "type": "LinguisticObject"
    },
    {
      "classified_as": [
        "https://example.org/type/C46_2"
      ],
      "id": "https://example.org/event/C46_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C47_1"
      ]
    },
    {
      "classified_as": [
        "https://example.org/type/C44_2"
      ],
      "id": "https://example.org/event/C44_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C45_1"
      ]
    },
    {
      "classified_as": [
        "https://example.org/type/C17_2"
      ],
      "id": "https://example.org/event/C17_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C18_1"
      ]
    },
    {
      "assigned_by": [
        "https://example.org/event/C46_1"
      ],
      "id": "https://example.org/place/fie_60_1",
      "type": "Place"
    },
    {
      "assigned_by": [
        "https://example.org/event/C44_1"
      ],
      "begin_of_the_begin": "",
      "end_of_the_end": "",
      "id": "https://example.org/time_span/fie_58_2",
      "type": "TimeSpan"
    },
    {
      "id": "https://example.org/time_span/fie_62_2",
      "type": "TimeSpan"
    },
    {
      "classified_as": [
        "https://example.org/type/C8_1"
      ],
      "crm:P01i_is_domain_of": {
        "id": "https://example.org/property/C16_1"
      },
      "id": "https://example.org/event/fie_62_1",
      "timespan": "https://example.org/time_span/fie_62_2",
      "type": [
        "Destruction",
        "Activity"
      ]
    }
  ]
}
                
```                

## Antique Monument **Substance**
The analysis and understanding of a *Antique Monument* depends also on our knowledge of its materiality and physical characteristics. The category of substance brings together descriptors which are relevant to this form of analysis. Particularly, it groups information having to do with the composition and measurable aspects of the *Antique Monument* as an object. 

| Filed ID    | Name                         | Description | Data Type | CRM Path |
| ----------- |------------------------------|-------------|-----------|----------| 
| fie_90   | Monument Material|    This field is used to record the material of which the documented *Antique Monument* consists. | Concept  |  --> P45 --> E57[90_1] |   
|fie_cen_82 |   Monument Material Uncertainty|    This field is used to record the concept of uncertainty defining the material of the documented *Antique Monument*.  |  Collection [Uncertainty] |   --> P45 --> E57[90_1] --> P141i --> E13[C82_1] |   
|fie_87 |   Monument Dimension Value  |  This field is used to record the value of the measured dimension of the documented *Antique Monument*.  |  Integer |   --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P90 --> xsd:decimal   | 
|fie_cen_91  |  Monument Dimension Verbatim  |  This field is used to record a verbatim describing the dimensions of the documented *Antique Monument*. |    String |   --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P67i --> E33_41[C91_1] --> P190 --> rdfs:literal    |
|fie_88 |   Monument Dimension Unit |   This field is used to record the unit of the measured dimension of the documented *Antique Monument*. |   Concept |   --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P91 --> E58[88_1]   | 
|fie_86 |   Monument Dimension Type  |  This field is used to record the type of measurement that the dimension of the documented *Antique Monument* represents.  |  Concept | --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P2 --> E55[86_3] |   
|fie_cen_55 |   Monument Dimension Statement |   This field is used to record the textual content of a statement made about the dimensions of the documented *Antique Monument*. |   String |   --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P67i --> E33_41[C55_1] --> P190 --> rdfs:literal    |

### - Antique Monument Substance **Ontology Graph**
![Screenshot](img/sub_monument.png)

### - Antique Monument Substance **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P39i_was_measured_by <https://example.org/event/fie_86_1> ;
    crm:P45_consists_of <https://example.org/type/material/fie_90_1> .

<https://example.org/appellation/C55_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P190_has_symbolic_content "dimension statement" .

<https://example.org/appellation/C91_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P190_has_symbolic_content "dimension verbatim" .

<https://example.org/dimension/fie_86_2> a crm:E54_Dimension ;
    crm:P2_has_type <https://example.org/type/fie_86_3> ;
    crm:P67i_is_referred_by <https://example.org/appellation/C55_1>,
        <https://example.org/appellation/C91_1> ;
    crm:P90_has_value "content" ;
    crm:P91_has_unit <https://example.org/type/fie_88_1> .

<https://example.org/event/C82_1> a crm:E13_Attribute_Assignment .

<https://example.org/event/fie_86_1> a crm:E16_Measurement ;
    crm:P40_observed_dimension <https://example.org/dimension/fie_86_2> .

<https://example.org/type/fie_86_3> a crm:E55_Type .

<https://example.org/type/fie_88_1> a crm:E58_Measurement_Unit .

<https://example.org/type/material/fie_90_1> a crm:E57_Material ;
    crm:P141i_was_assigned_by <https://example.org/event/C82_1> .

```

### - Antique Monument Substance **JSON-LD**                
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/event/C82_1",
      "type": "AttributeAssignment"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_86_3"
      ],
      "crm:P67i_is_referred_by": [
        {
          "id": "https://example.org/appellation/C55_1"
        },
        {
          "id": "https://example.org/appellation/C91_1"
        }
      ],
      "id": "https://example.org/dimension/fie_86_2",
      "type": "Dimension",
      "unit": "https://example.org/type/fie_88_1",
      "value": "content"
    },
    {
      "id": "https://example.org/type/fie_86_3",
      "type": "Type"
    },
    {
      "id": "https://census.de/example/physical_object/E22",
      "made_of": [
        "https://example.org/type/material/fie_90_1"
      ],
      "measured_by": [
        "https://example.org/event/fie_86_1"
      ],
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/event/fie_86_1",
      "observed_dimension": [
        "https://example.org/dimension/fie_86_2"
      ],
      "type": "Measurement"
    },
    {
      "assigned_by": [
        "https://example.org/event/C82_1"
      ],
      "id": "https://example.org/type/material/fie_90_1",
      "type": "Material"
    },
    {
      "id": "https://example.org/type/fie_88_1",
      "type": "MeasurementUnit"
    },
    {
      "content": "dimension verbatim",
      "id": "https://example.org/appellation/C91_1",
      "type": "Name"
    },
    {
      "content": "dimension statement",
      "id": "https://example.org/appellation/C55_1",
      "type": "Name"
    }
  ]
}
                
```                
## Antique Monument **Events**
This information category brings together typical events in which a *Antique Monument* may have been involved through the course of its history. It is meant to cover information concerning the most salient events documented with regards to *Antique Monuments*. At present this enables the documentation of provenance and preservation events.

| Filed ID    | Name                         | Description | Data Type | CRM Path |
| ----------- |------------------------------|-------------|-----------|----------| 
|fie_107   | Monument Preservation Event Type|    This field is used to record the type of preservation event performed on the documented *Antique Monument*. |    Concept |   --> P31i --> E11[107_1] --> P2 --> E55[107_2]|
|fie_cen_95  |  Monument Conservator   | This field is used to record a conservator who has conserved the documented *Antique Monument*.   | Reference Model [Person/Group] |  --> P31i --> E11[107_1] --> P01 --> PC14[C50_1] --> P02 --> E39[C95_1]|
|fie_cen_50  |  Monument Preservation Event Actor Role |   This field is used to record the specific role of the actor carried out the preservation event performed on the documented *Antique Monument*.    | Concept  |  --> P31i --> E11[107_1] --> P01 --> PC14[C50_1] --> P14.1 --> E55[C50_2]|
|fie_cen_48  |  Monument Preservation Event Actor Attribution  |  This field is used to record the type of attribution (Renaissance or contemporary) assigning the actor carried out the preservation event performed on the documented *Antique Monument*.  |  Concept  |  --> P31i --> E11[107_1] --> P01 --> PC14[C50_1]  --> P02 --> E39[C95_1] --> P141i -->E13[C48_1] --> P2 --> E55[C48_2]|
|fie_cen_101  |  Monument Conservation Period  |  This field is used to record the period during which a preservation event performed on the documented *Antique Monument* has happened.  |   Reference Model [Period]|   --> P31i --> E11[107_1]  --> P10 --> E4 [C101_1]|
|fie_cen_49  |  Monument Preservation Actor Source |   This field is used to relate a document carrying a textual reference about the attribution (Renaissance or contemporary) assigning the actor carried out the preservation event performed on the documented *Antique Monument* and the documented *Antique Monument* itself. |   Reference Model [Document]|   --> P31i --> E11[107_1] --> P01 --> PC14[C50_1]  --> P02 --> E39[C95_1] --> P141i -->E13[C48_1] --> P16 -->E33[C49_1] --> P128i --> E22[C49_2]|
|fie_cen_34  |  Monument Preservation Event Date  |  This field is used to record the overall timespan of a preservation event performed on the documented *Antique Monument*.   |  Collection [Timespan]|   --> P31i --> E11[107_1] --> P4 --> E52[108_1]|
|fie_cen_51  |  Monument Preservation Event Location  |   This field is used to record the place where  the preservation event performed on the documented *Antique Monument* was carried out.|    Reference Model  [Location]|  --> P31i --> E11[107_1] --> P7 --> E53[C51_1]|
|fie_cen_52 |   Monument Preservation Event Location Attribution  |  This field is used to record the type of attribution (Renaissance or contemporary) assigning the place where the preservation event performed on the documented *Antique Monument* was carried out.   | Concept |   --> P31i --> E11[107_1] --> P7 --> E53[C51_1] --> P141i -->E13[C52_1] --> P2 --> E55[C52_2]|
|fie_cen_53  |  Monument Preservation Event Location Source  |  This field is used to relate a document carrying a textual reference about the type of attribution (Renaissance or contemporary) assigning the place where the preservation event performed on the documented *Antique Monument* was carried out and the documented *Antique Monument* itself.  |  Reference Model [Document]|   --> P31i --> E11[107_1] --> P7 --> E53[C51_1] --> P141i -->E13[C52_1]  --> P16 -->E33[C53_1] --> P128i --> E22[C53_2]|
|fie_cen_41  |  Monument Preservation Event Comments  |  This field is used to record a general statement about a preservation event performed on the documented *Antique Monument*.   |  Collection  [Statement]|  --> P31i --> E11[107_1] --> P67i --> E33[C41_1]|
|fie_269  |  Monument Provenance Event Type  |  This field is used to indicate the type of a provenance activity associated with the documented *Antique Monument*.   | Concept  |  --> P16i --> E7[268_1] --> P2 --> E55[269_1]|
|fie_cen_98 |   Monument Provenance Event Actor  |  This field is used to record the actor participated in a provenance activity associated with the documented *Antique Monument*.  |  Reference Model   [Person/Group]| --> P16i --> E7[268_1] --> P01i --> PC14[C70_1] --> P02 --> E39[C98_1]|
|fie_cen_70  |  Monument Provenance Event Actor Role |   This field is used to indicate the specific role of the actor carried out the provenance activity associated with the documented *Antique Monument*. |   Concept  |  --> P16i --> E7[268_1] --> P01 --> PC14[C70_1] --> P14.1 --> E55[C70_2]|
|fie_cen_71  |  Monument Provenance Event Actor Attribution |   This field is used to record the type of attribution (Renaissance or contemporary) assigning the actor carried out the provenance activity associated with the documented *Antique Monument*.   | Concept   | --> P16i --> E7[268_1] --> P01 --> PC14[C70_1] --> P02 --> E39[C98_1] --> P141i -->E13[C71_1] --> P2 --> E55[C71_2]|
|fie_cen_72  |  Monument Provenance Event Actor Source  |  This field is used to record the document carrying a textual reference about the type of attribution (renaissance or contemporary) assigning the actor carried out the provenance activity associated with the documented *Antique Monument* and the documented *Antique Monument* itself.   | Reference Model  [Document]|  --> P16i --> E7[268_1] --> P01 --> PC14[C70_1] --> P02 --> E39[C98_1] --> P141i -->E13[C71_1] --> P16 -->E33[C72_1] --> P128i -->E22[C72_2]|
|fie_cen_68 |   Monument Provenance Event Date |   This field is used to record the timespan of a provenance activity associated with the documented *Antique Monument*.  |  Collection [Timespan]|   --> P16i --> E7[268_1] --> P4 --> E52[270_1] |
|fie_cen_73 |   Monument Provenance Event Location  |  This field is used to record the location of the provenance activity associated with the documented *Antique Monument*.  |  Reference Model [Location]|   --> P16i --> E7[268_1] --> P7 --> E53[C73_1]|
|fie_cen_75  |  Monument Provenance Event Location Source |   This field is used to relate the document carrying a textual reference about the type of attribution (renaissance or contemporary) assigning the location of the provenance activity associated with the documented *Antique Monument* and the document *Antique Monument* itself.  |  Reference Model [Document]|   --> P16i --> E7[268_1] --> P7 --> E53[C73_1] --> P141i -->E13[C74_1] --> P16 -->E33[C75_1] --> P128i -->E22[C75_2]|
|fie_cen_74 |   Monument Provenance Event Location Attribution |   This field is used to record the type of attribution (Renaissance or contemporary) assigning the location of the provenance activity associated with the documented *Antique Monument*.  |  Concept  |  --> P16i --> E7[268_1] --> P7 --> E53[C73_1] --> P141i -->E13[C74_1] --> P2 --> E55[C74_2]|
|fie_cen_76 |   Monument Provenance Event Notes |   This field is used to record a general statement about the provenance activity associated with the documented *Antique Monument*. |   Collection  [Statement]|  --> P16i --> E7[268_1] --> P67i --> E33[C76_1]|
|fie_cen_100 |   Monument Preservation Event Period  |  This field is used to record the period during which a provenance activity associated with the documented *Antique Monument* has happened.  |  Reference Model  [Period]|  --> P16i --> E7[268_1] --> P10 --> E4 [C100_1]|

### - Antique Monument Events **Ontology Graph**
![Screenshot](img/ev_monument.png)

### - Antique Monument Events **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P16i_was_used_for <https://example.org/event/fie_268_1> ;
    crm:P31i_was_modified_by <https://example.org/event/fie_107_1> .

<https://example.org/actor/C95_1> a crm:E39_Actor ;
    crm:P141i_was_assigned_by <https://example.org/event/C48_1> .

<https://example.org/actor/C98_1> a crm:E39_Actor ;
    crm:P141i_was_assigned_by <https://example.org/event/C71_1> .

<https://example.org/conceptual_object/C41_1> a crm:E33_Linguistic_Object .

<https://example.org/conceptual_object/C49_1> a crm:E33_Linguistic_Object ;
    crm:P128i_carried_by <https://example.org/physical_object/C49_2> .

<https://example.org/conceptual_object/C53_1> a crm:E33_Linguistic_Object ;
    crm:P128i_carried_by <https://example.org/physical_object/C53_2> .

<https://example.org/conceptual_object/C72_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C72_2> .

<https://example.org/conceptual_object/C75_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C75_2> .

<https://example.org/conceptual_object/C76_1> a crm:E33_Linguistic_Object .

<https://example.org/event/C48_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C49_1> ;
    crm:P2_has_type <https://example.org/type/C48_2> .

<https://example.org/event/C52_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C53_1> ;
    crm:P2_has_type <https://example.org/type/C52_2> .

<https://example.org/event/C71_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C72_1> ;
    crm:P2_has_type <https://example.org/type/C71_2> .

<https://example.org/event/C74_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C75_1> ;
    crm:P2_has_type <https://example.org/type/C74_2> .

<https://example.org/event/fie_107_1> a crm:E11_Modification ;
    crm:P01i_is_domain_of <https://example.org/property/C50_1> ;
    crm:P10_falls_within <https://example.org/period/C101_1> ;
    crm:P2_has_type <https://example.org/type/fie_107_2> ;
    crm:P4_has_time-span <https://example.org/time_span/fie_108_1> ;
    crm:P67i_was_referred_to_by <https://example.org/conceptual_object/C41_1> ;
    crm:P7_took_place_at <https://example.org/place/C51_1> .

<https://example.org/event/fie_268_1> a crm:E7_Activity ;
    crm:P01i_is_domain_of <https://example.org/property/C70_1> ;
    crm:P10_falls_within <https://example.org/period/C100_1> ;
    crm:P2_has_type <https://example.org/type/fie_269_1> ;
    crm:P4_has_time-span <https://example.org/time_span/fie_270_1> ;
    crm:P67i_is_referred_to_by <https://example.org/conceptual_object/C76_1> ;
    crm:P7_took_place_at <https://example.org/place/C73_1> .

<https://example.org/period/C100_1> a crm:E4_Period .

<https://example.org/period/C101_1> a crm:E4_Period .

<https://example.org/physical_object/C49_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C53_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C72_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C75_2> a crm:E22_Human-Made_Object .

<https://example.org/place/C51_1> a crm:E53_Place ;
    crm:P141i_was_assigned_by <https://example.org/event/C52_1> .

<https://example.org/place/C73_1> a crm:E53_Place ;
    crm:P141i_was_assigned_by <https://example.org/event/C74_1> .

<https://example.org/property/C50_1> a crm:PC14_carried_out_by ;
    crm:P02_has_range <https://example.org/actor/C95_1> ;
    crm:P14.1_in_the_role_of <https://example.org/type/C50_2> .

<https://example.org/property/C70_1> a crm:PC14_carried_out_by ;
    crm:P02_has_range <https://example.org/actor/C98_1> ;
    crm:P14.1_in_the_role_of <https://example.org/type/C70_2> .

<https://example.org/time_span/fie_108_1> a crm:E52_Time-Span .

<https://example.org/time_span/fie_270_1> a crm:E52_Time-Span .

<https://example.org/type/C48_2> a crm:E55_Type .

<https://example.org/type/C50_2> a crm:E55_Type .

<https://example.org/type/C52_2> a crm:E55_Type .

<https://example.org/type/C70_2> a crm:E55_Type .

<https://example.org/type/C71_2> a crm:E55_Type .

<https://example.org/type/C74_2> a crm:E55_Type .

<https://example.org/type/fie_107_2> a crm:E55_Type .

<https://example.org/type/fie_269_1> a crm:E55_Type .


```
### - Antique Monument Events **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://census.de/example/physical_object/E22",
      "modified_by": [
        "https://example.org/event/fie_107_1"
      ],
      "type": "HumanMadeObject",
      "used_for": [
        "https://example.org/event/fie_268_1"
      ]
    },
    {
      "id": "https://example.org/type/C52_2",
      "type": "Type"
    },
    {
      "crm:P02_has_range": {
        "id": "https://example.org/actor/C98_1"
      },
      "crm:P14.1_in_the_role_of": {
        "id": "https://example.org/type/C70_2"
      },
      "id": "https://example.org/property/C70_1",
      "type": "crm:PC14_carried_out_by"
    },
    {
      "assigned_by": [
        "https://example.org/event/C48_1"
      ],
      "id": "https://example.org/actor/C95_1",
      "type": "Actor"
    },
    {
      "id": "https://example.org/period/C100_1",
      "type": "Period"
    },
    {
      "assigned_by": [
        "https://example.org/event/C71_1"
      ],
      "id": "https://example.org/actor/C98_1",
      "type": "Actor"
    },
    {
      "id": "https://example.org/period/C101_1",
      "type": "Period"
    },
    {
      "id": "https://example.org/time_span/fie_270_1",
      "type": "TimeSpan"
    },
    {
      "crm:P128i_carried_by": {
        "id": "https://example.org/physical_object/C53_2"
      },
      "id": "https://example.org/conceptual_object/C53_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/C70_2",
      "type": "Type"
    },
    {
      "crm:P128i_carried_by": {
        "id": "https://example.org/physical_object/C49_2"
      },
      "id": "https://example.org/conceptual_object/C49_1",
      "type": "LinguisticObject"
    },
    {
      "carried_by": [
        "https://example.org/physical_object/C75_2"
      ],
      "id": "https://example.org/conceptual_object/C75_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/C50_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/physical_object/C49_2",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/conceptual_object/C76_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/C48_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/time_span/fie_108_1",
      "type": "TimeSpan"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_269_1"
      ],
      "crm:P01i_is_domain_of": {
        "id": "https://example.org/property/C70_1"
      },
      "falls_within": [
        "https://example.org/period/C100_1"
      ],
      "id": "https://example.org/event/fie_268_1",
      "referred_to_by": [
        "https://example.org/conceptual_object/C76_1"
      ],
      "timespan": "https://example.org/time_span/fie_270_1",
      "took_place_at": [
        "https://example.org/place/C73_1"
      ],
      "type": "Activity"
    },
    {
      "assigned_by": [
        "https://example.org/event/C74_1"
      ],
      "id": "https://example.org/place/C73_1",
      "type": "Place"
    },
    {
      "id": "https://example.org/physical_object/C72_2",
      "type": "HumanMadeObject"
    },
    {
      "classified_as": [
        "https://example.org/type/C74_2"
      ],
      "id": "https://example.org/event/C74_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C75_1"
      ]
    },
    {
      "id": "https://example.org/type/fie_107_2",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/type/C52_2"
      ],
      "id": "https://example.org/event/C52_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C53_1"
      ]
    },
    {
      "id": "https://example.org/conceptual_object/C41_1",
      "type": "LinguisticObject"
    },
    {
      "classified_as": [
        "https://example.org/type/C71_2"
      ],
      "id": "https://example.org/event/C71_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C72_1"
      ]
    },
    {
      "id": "https://example.org/physical_object/C75_2",
      "type": "HumanMadeObject"
    },
    {
      "classified_as": [
        "https://example.org/type/C48_2"
      ],
      "id": "https://example.org/event/C48_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C49_1"
      ]
    },
    {
      "id": "https://example.org/type/fie_269_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/physical_object/C53_2",
      "type": "HumanMadeObject"
    },
    {
      "carried_by": [
        "https://example.org/physical_object/C72_2"
      ],
      "id": "https://example.org/conceptual_object/C72_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/C74_2",
      "type": "Type"
    },
    {
      "crm:P02_has_range": {
        "id": "https://example.org/actor/C95_1"
      },
      "crm:P14.1_in_the_role_of": {
        "id": "https://example.org/type/C50_2"
      },
      "id": "https://example.org/property/C50_1",
      "type": "crm:PC14_carried_out_by"
    },
    {
      "id": "https://example.org/type/C71_2",
      "type": "Type"
    },
    {
      "assigned_by": [
        "https://example.org/event/C52_1"
      ],
      "id": "https://example.org/place/C51_1",
      "type": "Place"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_107_2"
      ],
      "crm:P01i_is_domain_of": {
        "id": "https://example.org/property/C50_1"
      },
      "crm:P67i_was_referred_to_by": {
        "id": "https://example.org/conceptual_object/C41_1"
      },
      "falls_within": [
        "https://example.org/period/C101_1"
      ],
      "id": "https://example.org/event/fie_107_1",
      "timespan": "https://example.org/time_span/fie_108_1",
      "took_place_at": [
        "https://example.org/place/C51_1"
      ],
      "type": "Modification"
    }
  ]
}
                
```                

## Antique Monument **Designation Status**
Characteristic of information gathered relative to *Antique Monuments* are various kinds of official designations types that are given to these objects by various agencies. Assignment of such designations is related to various protocols in the assigning institutions and are often accompanied by regulations on the kind of activity that can be undertaken relative to the built work in question. Such designations also provide means of identifying a *Antique Monument* across records. This information category gathers together descriptors relative to this information.

| Filed ID    | Name                         | Description | Data Type | CRM Path |
| ----------- |------------------------------|-------------|-----------|----------| 
|fie_cen_14  |  Monument Condition State Moment |   This field is used to record the state moment (original/present)  of the condition assessment of the documented *Antique Monument*. |   Concept  |  --> P44 --> E3[255_1] --> P34i --> E14[256_1] --> P2 --> E55[C14_1]  |  
|fie_255  |  Monument Condition State Type |   This field is used to indicate the type of a condition state that has been attributed to the documented *Antique Monument*. |   Concept  |  --> P44 --> E3[255_1] --> P2 --> E55[255_2] |   
|fie_cen_85 |   Monument Condition State Uncertainty |   This field is used to record the concept of uncertainty defining the condition state of the documented *Antique Monument*.  |  Collection [Uncertainty]  |  --> P44 --> E3[255_1] --> P2 --> E55[255_2] --> P141i --> E13[C85_1]   | 
|fie_cen_11   | Monument Condition Actor Role |   This field is used to record the specific role of the actor carried out the the condition assessment of the documented *Antique Monument*.  |  Concept  |  --> P44 --> E3[255_1] --> P34i --> E14[256_1] --> P01 --> PC14[C11_1] --> P14.1 --> E55[C11_2] | 
|fie_258  |  Monument Condition Earliest Date |   This field is used to record the earliest possible date for the condition assessment of the documented *Antique Monument*.|    Date  |  --> P44 --> E3[255_1] --> P34i --> E14[256_1] --> P4 --> E52[258_1] --> P82a --> xsd:dateTime    |
|fie_259  |  Monument Condition Latest Date |   This field is used to record the latest possible date for the condition assessment of the documented *Antique Monument*. |   Date  |  --> P44 --> E3[255_1] --> P34i --> E14[256_1] --> P4 --> E52[258_1] --> P82b --> xsd:dateTime   | 
|fie_cen_10 |   Monument Condition Falls Within  |  This field is used to record the period during in which a condition assessment of the documented *Antique Monument* occurred. |  Reference Model [Period] |   --> P44 --> E3[255_1] --> P34i --> E14[256_1] --> P10 --> E4[C10_1]    |
|fie_cen_12  |  Monument Condition Source |   This field is used to relate the condition assessment of the documented *Antique Monument* and a document carrying a textual reference about reference about the condition assessment of the documented *Antique Monument*. |  Reference Model [Document] |   --> P44 --> E3[255_1] --> P34i --> E14[256_1] --> P141i --> E13[C12_1] --> P16 --> E33[C12_2] --> P128i --> E22[C12_3]  |  

### - Antique Monument Designation Status **Ontology Graph**
![Screenshot](img/des_monument.png)

### - Antique Monument Designation Status **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix xsd: <http://www.w3.org/2001/XMLSchema#> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P44_has_condition <https://example.org/event/fie_255_1> .

<https://example.org/conceptual_object/C12_2> a crm:E33_Linguistic_Object .

<https://example.org/event/C85_1> a crm:E13_Attribute_Assignment .

<https://example.org/event/fie_255_1> a crm:E3_Condition_State ;
    crm:P2_has_type <https://example.org/type/fie_255_2> ;
    crm:P34i_was_assessed_by <https://example.org/event/fie_256_1> .

<https://example.org/event/fie_256_1> a crm:E14_Condition_Assessment ;
    crm:P01i_is_domain_of <https://example.org/property/C11_1> ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C12_2> ;
    crm:P2_has_type <https://example.org/type/C14_1> ;
    crm:P4_has_time-span <https://example.org/time_span/fie_258_1> .

<https://example.org/period/C10_1> a crm:E4_Period .

<https://example.org/property/C11_1> a crm:PC14_carried_out_by ;
    crm:P14.1_in_the_role_of <https://example.org/type/C11_2> .

<https://example.org/time_span/fie_258_1> a crm:E52_Time-Span ;
    crm:P10_falls_within <https://example.org/period/C10_1> ;
    crm:P82a_begin_of_the_begin ""^^xsd:dateTime ;
    crm:P82b_end_of_the_end ""^^xsd:dateTime .

<https://example.org/type/C11_2> a crm:E55_Type .

<https://example.org/type/C14_1> a crm:E55_Type .

<https://example.org/type/fie_255_2> a crm:E55_Type ;
    crm:P141i_was_assigned_by <https://example.org/event/C85_1> .

```
                
### - Antique Monument Designation Status **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "classified_as": [
        "https://example.org/type/C14_1"
      ],
      "crm:P01i_is_domain_of": {
        "id": "https://example.org/property/C11_1"
      },
      "id": "https://example.org/event/fie_256_1",
      "timespan": "https://example.org/time_span/fie_258_1",
      "type": "ConditionAssessment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C12_2"
      ]
    },
    {
      "id": "https://example.org/period/C10_1",
      "type": "Period"
    },
    {
      "crm:P14.1_in_the_role_of": {
        "id": "https://example.org/type/C11_2"
      },
      "id": "https://example.org/property/C11_1",
      "type": "crm:PC14_carried_out_by"
    },
    {
      "condition": [
        "https://example.org/event/fie_255_1"
      ],
      "id": "https://census.de/example/physical_object/E22",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/conceptual_object/C12_2",
      "type": "LinguisticObject"
    },
    {
      "assigned_by": [
        "https://example.org/event/C85_1"
      ],
      "id": "https://example.org/type/fie_255_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/C14_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/event/C85_1",
      "type": "AttributeAssignment"
    },
    {
      "begin_of_the_begin": "",
      "end_of_the_end": "",
      "falls_within": [
        "https://example.org/period/C10_1"
      ],
      "id": "https://example.org/time_span/fie_258_1",
      "type": "TimeSpan"
    },
    {
      "id": "https://example.org/type/C11_2",
      "type": "Type"
    },
    {
      "assessed_by": [
        "https://example.org/event/fie_256_1"
      ],
      "classified_as": [
        "https://example.org/type/fie_255_2"
      ],
      "id": "https://example.org/event/fie_255_1",
      "type": "ConditionState"
    }
  ]
}
                
```                
## Antique Monument **Location**
The documentation of location aids in tracking the present location of individual *Antique Monuments* as well their dispersion geographically. This information category gathers together relevant descriptors for this task.

| Filed ID    | Name                         | Description | Data Type | CRM Path |
| ----------- |------------------------------|-------------|-----------|----------|
|fie_177   | Monument Current Location  |  This field is used to record the address at which the documented instance of *Antique Monument* is located.  |  String |   --> P53 --> E53[177_1] --> P1 --> E41[177_2]<br><br>P53 --> E53[177_1] --> P1 --> E41[177_2] --> P2 --> E55 "Address"[177_3]|

### - Antique Monument Location **Ontology Graph**
![Screenshot](img/loc_monument.png)

### - Antique Monument Location **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P53_has_former_or_current_location <https://example.org/place/fie_177_1> .

<https://example.org/name/fie_177_2> a crm:E41_Appellation ;
    crm:P2_has_type <https://example.org/type/fie_177_3> .

<https://example.org/place/fie_177_1> a crm:E53_Place ;
    crm:P1_is_identified_by <https://example.org/name/fie_177_2> .

<https://example.org/type/fie_177_3> a crm:E55_Type ;
    rdfs:label "Address" .
```

 ### - Antique Monument Location **JSON-LD**               
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "former_or_current_location": [
        "https://example.org/place/fie_177_1"
      ],
      "id": "https://census.de/example/physical_object/E22",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/place/fie_177_1",
      "identified_by": [
        "https://example.org/name/fie_177_2"
      ],
      "type": "Place"
    },
    {
      "_label": "Address",
      "id": "https://example.org/type/fie_177_3",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_177_3"
      ],
      "id": "https://example.org/name/fie_177_2",
      "type": "Appellation"
    }
  ]
}
```                
## Antique Monument **Description**
*Antique Monuments* are the subjects of innumerable descriptions that provide a wide range of information with regards to the aesthetic and historical importance of the work, inter alia. Such descriptions are of use in a scholarly understanding of a *Antique Monument* just in case we are able to track the provenance of such elocutions in a systematic fashion. Such an aim drives the need for the tracking of description information as a separate category. The descriptors necessary to this task are documented in the table below.

| Filed ID    | Name                         | Description | Data Type | CRM Path |
| ----------- |------------------------------|-------------|-----------|----------|
|fie_cen_31  |  Monument Relations  |  This field is used to record the similarity between the documented monument and another *Antique Monument*.  | Reference Model [Monument] |   --> P01i --> PC130[C31_1] --> P02 --> E22[C31_2] |
|fie_cen_32 |   Monument Relation Type  |  This field is used to record the type of similarity between the documented *Antique Monument* and another *Antique Monument*. |    Concept  |  --> P01i --> PC130[C31_1] --> P130.1 --> E55[C32_1] |
|fie_cen_58  |  Monument Notes  |  This field is used to record a general statement made about the documented *Antique Monument*.  |  Collection [Statement] |   --> P67i --> E33[C58_1] |

### - Antique Monument Description **Ontology Graph**
![Screenshot](img/desc_monument.png)

### - Antique Monument Description **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P01i_is_domain_of <https://example.org/reified_property/C31_1> ;
    crm:P67i_is_referred_to_by <https://example.org/conceptual_object/C58_1> .

<https://example.org/conceptual_object/C58_1> a crm:E33_Linguistic_Object .

<https://example.org/physical_object/C31_2> a crm:E22_Human-made_Object .

<https://example.org/reified_property/C31_1> a crm:PC130_shows_features_of ;
    crm:PC02_has_range <https://example.org/physical_object/C31_2> ;
    crm:PC130.1_has_type <https://example.org/type/C32_1> .

<https://example.org/type/C32_1> a crm:E55_Type .
```
### - Antique Monument Description **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/physical_object/C31_2",
      "type": "crm:E22_Human-made_Object"
    },
    {
      "id": "https://example.org/type/C32_1",
      "type": "Type"
    },
    {
      "crm:P01i_is_domain_of": {
        "id": "https://example.org/reified_property/C31_1"
      },
      "id": "https://census.de/example/physical_object/E22",
      "referred_to_by": [
        "https://example.org/conceptual_object/C58_1"
      ],
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/conceptual_object/C58_1",
      "type": "LinguisticObject"
    },
    {
      "crm:PC02_has_range": {
        "id": "https://example.org/physical_object/C31_2"
      },
      "crm:PC130.1_has_type": {
        "id": "https://example.org/type/C32_1"
      },
      "id": "https://example.org/reified_property/C31_1",
      "type": "crm:PC130_shows_features_of"
    }
  ]
}
```                
## Antique Monument **Documentation**
This information category unites referential information about the documented *Antique Monument*, providing contextual data about it.

| Filed ID    | Name                         | Description | Data Type | CRM Path |
| ----------- |------------------------------|-------------|-----------|----------|
|fie_196 |   Monument Citation |   This field is used to record a citation to reference documentation for the documented *Antique Monument*.  |  String  |  --> P129i --> E33[196_1] --> rdf:value --> rdfs:Literal<br><br>--> P129i --> E33[196_1] --> P2 --> E55 "Citation" |
|fie_197 |   Monument Citation Source |   This field is used to record the source used for generating the citation for the documented *Antique Monument*. |   Reference Model [Bibliographic Entity] |    --> P129i --> E33[196_1] --> P106i --> E33[197_1]|
|fie_cen_24 |   Monument Document Reference  |  This field is used to record the source used for generating the citation for the documented *Antique Monument*. |  Reference Model [Document] |  --> P67i --> E33[C24_1] --> P128i --> E22[C24_2]|
|fie_195  |  Monument Image  |  This field is used to record a digital image which is representative of the documented *Antique Monument*.  |   Reference Model [Image] |   --> P138i --> E36/D9[195_1]|
|fie_204 |   Monument URL  |  The field is used to record the sameness between the *Antique Monument* described and an external authority. |   uri  |  --> L54 --> E1[204_1]
|fie_cen_57  |  Monument URL Title  |  This field is used to record a title of an external digital authority related to the documented *Antique Monument*. |    String   | --> L54 --> E1[204_1] --> P1 --> E33_E41[C57_1]|

### - Antique Monument Documentation **Ontology Graph**
![Screenshot](img/doc_monument.png)

### - Antique Monument Documentation **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:L54_is_same-as <https://example.org/entity/fie_204_1> ;
    crm:P129i_is_subject_of <https://example.org/conceptual_object/fie_196_1> ;
    crm:P138i_has_representation <https://example.org/conceptual_object/fie_195_1> ;
    crm:P67i_is_referred_to_by <https://example.org/conceptual_object/C24_1> .

<https://example.org/appellation/C57_1> a crm:E33_E41_Linguistic_Appellation .

<https://example.org/conceptual_object/C24_1> a crm:E33_Lingusitic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C24_2> .

<https://example.org/conceptual_object/fie_195_1> a crm:D9_Data_Object,
        crm:E36_Visual_Item .

<https://example.org/conceptual_object/fie_196_1> a crm:E33_Linguistic_Object ;
    crm:P106i_forms_part_of <https://example.org/conceptual_object/fie_197_1> ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <https://example.org/type/fie_196_1> .

<https://example.org/conceptual_object/fie_197_1> a crm:E33_Linguistic_Object .

<https://example.org/entity/fie_204_1> a crm:E1_CRM_Entity ;
    crm:P1_is_identified_by <https://example.org/appellation/C57_1> .

<https://example.org/physical_object/C24_2> a crm:E22_Human-Made_Object .

<https://example.org/type/fie_196_1> a crm:E55_Type ;
    rdfs:label "Citation" .
```
### - Antique Monument Documentation **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/entity/fie_204_1",
      "identified_by": [
        "https://example.org/appellation/C57_1"
      ],
      "type": "CRMEntity"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_196_1"
      ],
      "content": "content",
      "crm:P106i_forms_part_of": {
        "id": "https://example.org/conceptual_object/fie_197_1"
      },
      "id": "https://example.org/conceptual_object/fie_196_1",
      "type": "LinguisticObject"
    },
    {
      "crm:L54_is_same-as": {
        "id": "https://example.org/entity/fie_204_1"
      },
      "id": "https://census.de/example/physical_object/E22",
      "referred_to_by": [
        "https://example.org/conceptual_object/C24_1"
      ],
      "representation": [
        "https://example.org/conceptual_object/fie_195_1"
      ],
      "subject_of": [
        "https://example.org/conceptual_object/fie_196_1"
      ],
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/conceptual_object/fie_195_1",
      "type": [
        "VisualItem",
        "crm:D9_Data_Object"
      ]
    },
    {
      "id": "https://example.org/conceptual_object/fie_197_1",
      "type": "LinguisticObject"
    },
    {
      "carried_by": [
        "https://example.org/physical_object/C24_2"
      ],
      "id": "https://example.org/conceptual_object/C24_1",
      "type": "crm:E33_Lingusitic_Object"
    },
    {
      "_label": "Citation",
      "id": "https://example.org/type/fie_196_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/physical_object/C24_2",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/appellation/C57_1",
      "type": "Name"
    }
  ]
}
```                
