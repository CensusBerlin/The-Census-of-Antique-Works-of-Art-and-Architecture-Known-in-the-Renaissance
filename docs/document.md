**Document**

**Author:** Denitsa Nenova, George Bruseker

**Version:** 1.0

The *Document* model is intended to enable the representation and sharing of data relevant to human-made, physical items – works of art (such as drawings, prints, statuettes, paintings or medals), or texts (such as inventories or guidebooks) – which carry content that provides evidence of a historical witnessing of or reference to a *Monument*. An instance of the *Document* model is typically a primary, physical artwork or text dating to the period of study (typically, the Renaissance as defined as the period between 1400 and 1600) that responds to or bears witness to a *Monument*. *Documents* are recorded as objects in and of themselves and are intended to trace assertions about, sightings of or responses to *Monuments*, allowing researchers to gain an understanding of the whole corpus of Renaissance knowledge of antique works of art and architecture. *Documents* also provide  opinions or perspectives on *Monuments*, not only with regard to the *Monument*’s identification, date, and condition,  but also with regard to the *Monument*’s cultural and symbolic significance, its artistic value, and its identity in a specific Renaissance setting and context.



| | Name| URI | 
|-|-----|-----|
|Root Ontology Node|E22 Human-Made Object | https://cidoc-crm.org/Entity/E22-Human-Made-Object/version-7.1.1|
|Type Differentiator |documents | http://vocab.getty.edu/aat/300026030 |

The *Document* model allows the documentation of the following kinds of information:

|Information Category | Information Collections | Description | 
|---------------------|-------------------------|-------------|
| Names and Classifications |   Names/Alternative Names/Identifiers/Type  |  The researcher can document various names and classification regarding the *Document*.|
|Existence   | Production/Destruction |   The researcher can document the events related to the production and destruction of a *Document*.|
|Events   | Provenance |   The researcher can document the events related to the provenance of a *Document*.|
|Substance   | Dimension/Material  | The researcher can document various physical information about the *Document*.|
|Aboutness   | Visual/Textual | The researcher can document the kind of visual or textual information that the *Document* is a bearer of.|
|Locations   | Location   | The researcher can document the location of the *Document*.|
|Description  |  Description |   The researcher can document various free-text descriptions of the *Document*.|
|Documentation  |  Citation/Image/External URI| The researcher can document citations relative to the *Document*, link to images of the *Document* and document external URIs of documentation for the same *Document*.|

## Document **Names and Classifications**

The attribution of names and types to *Document*, as with other entities, is a basic human activity. A chief factor in disambiguating *Documents* lies in understanding the various names and identifiers that have been given to them at different moments in their individual histories. Likewise, additional classifiers of the *Document* give important distinguishing characteristics.

| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_5  |  Document Name  |  This field is used to record the main name attributed to the described *Document*.  |  String  |  --> P1 --> E33_E41[5_1] --> P190 --> rdfs:Literal<br><br> --> P1 --> E33_E41[5_1] --> P2 --> E55[5_2]{'preferred terms'}|
|fie_10  |  Document Alias |   This field is used to record an alternative name under which the described *Document* is known.   |  String  |  --> P1 --> E33_E41[10_1]  --> P190 --> rdfs:Literal|
|fie_11   | Document Alias Type |   This field is used to record the type of the alternative name that has been attributed to the described *Document*.  |  Concept  |  --> P1 --> E33_E41[10_1] --> P2 --> E55[11_1]|
|fie_16  |  Document Alias Source    |This field is used to record the source on the basis of which the organization attributing the alternative name use based their attribution.  |  Reference Model [Bibliographic Entity/Image]|   --> P1 --> E33_E41[10_1] --> P141i --> E13[15_1] --> P16 --> E73[16_1]|
|fie_1  |  Document Identifier  |  This field is used to record an identifier attributed to the described *Document*. |   String  |  --> P1 --> E42[1_1] --> P190 --> rdfs:Literal|
|fie_2  |  Document Identifier Type |   This field is used to record the type of the identifier attributed to the described *Document*.  |  Concept |   --> P1 --> E42[1_1] --> P2 --> E55[2_1]|
|fie_3  |  Document ID Provider |   This field is used to record the institution, group or individual responsible for providing the described *Document*'s identifier.  |  Reference Model [Person/Group]|    --> P1 --> E42[1_1] --> P37i --> E15[3_1] --> P14 --> E39[3_2]|
|fie_4  |  Document ID Source  |  This field is used to record the institution, group or individual responsible for providing the described *Document*'s identifier.  |  Reference Model [Bibliographic Entity/Image]|   --> P1 --> E42[1_1] --> P37i --> E15[3_1] --> P16 --> E73[4_1]|
|fie_17 |   Document Type  |  This field is used to record the formal type of the described *Document*.  |  Concept  |  --> P2 --> E55[17_1]|
|fie_cen_86 |   Document Form  |  This field is used to record the concept of uncertainty defining the form of the described *Document*. |   Concept  |  --> P2 --> E55[86_1] --> P2 --> E55[86_2]|
|fie_cen_87 |   Document Representation Method  |  This field is used to record a statement about the representation method of the documented *Document*. |   Concept  |  --> P2 --> E55[87_1] --> P2 --> E55[87_2]|


### - Document Names and Classifications **Ontology Graph**
![Screenshot](img/nc_document.png)

### - Document Names and Classifications **RDF**

```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P1_is_identified_by <https://example.org/name/fie_10_1>,
        <https://example.org/name/fie_1_1>,
        <https://example.org/name/fie_5_1> ;
    crm:P2_has_type <https://example.org/type/C86_1>,
        <https://example.org/type/C87_1>,
        <https://example.org/type/fie_17_1> .

<http://vocab.getty.edu/aat/300404670> a crm:E55_Type ;
    rdfs:label "preferred terms" .

<https://example.org/actor/fie_3_2> a crm:E39_Actor .

<https://example.org/conceptual_object/fie_16_1> a crm:E73_Information_Object .

<https://example.org/conceptual_object/fie_4_1> a crm:E73_Information_Object .

<https://example.org/event/fie_15_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/fie_16_1> .

<https://example.org/event/fie_3_1> a crm:E15_Identifier_Assignment ;
    crm:P14_carried_out_by <https://example.org/actor/fie_3_2> ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/fie_4_1> .

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

<https://example.org/type/C86_1> a crm:E55_Type ;
    crm:P2_has_type <https://example.org/type/C86_2> .

<https://example.org/type/C86_2> a crm:E55_Type .

<https://example.org/type/C87_1> a crm:E55_Type ;
    crm:P2_has_type <https://example.org/type/C87_2> .

<https://example.org/type/C87_2> a crm:E55_Type .

<https://example.org/type/fie_11_1> a crm:E55_Type .

<https://example.org/type/fie_17_1> a crm:E55_Type .

<https://example.org/type/fie_2_1> a crm:E55_Type .


                
```

### - Document Names and Classifications **JOSN-LD**     
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/actor/fie_3_2",
      "type": "Actor"
    },
    {
      "classified_as": [
        "https://example.org/type/C86_2"
      ],
      "id": "https://example.org/type/C86_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/fie_2_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/conceptual_object/fie_16_1",
      "type": "InformationObject"
    },
    {
      "id": "https://example.org/event/fie_15_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/fie_16_1"
      ]
    },
    {
      "_label": "preferred terms",
      "id": "http://vocab.getty.edu/aat/300404670",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/type/C87_1",
        "https://example.org/type/fie_17_1",
        "https://example.org/type/C86_1"
      ],
      "id": "https://census.de/example/physical_object/E22",
      "identified_by": [
        "https://example.org/name/fie_1_1",
        "https://example.org/name/fie_5_1",
        "https://example.org/name/fie_10_1"
      ],
      "type": "HumanMadeObject"
    },
    {
      "classified_as": [
        "https://example.org/type/C87_2"
      ],
      "id": "https://example.org/type/C87_1",
      "type": "Type"
    },
    {
      "carried_out_by": [
        "https://example.org/actor/fie_3_2"
      ],
      "id": "https://example.org/event/fie_3_1",
      "type": "IdentifierAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/fie_4_1"
      ]
    },
    {
      "id": "https://example.org/type/fie_17_1",
      "type": "Type"
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
      "id": "https://example.org/type/fie_11_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/conceptual_object/fie_4_1",
      "type": "InformationObject"
    },
    {
      "id": "https://example.org/type/C87_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/C86_2",
      "type": "Type"
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
    }
  ]
}
                
```                           



## Document **Existence**
Of essential import in identifying and tracking documents is information pertaining to their existence in time, particularly information regarding the creation and destruction of the document. For this reason, we have clustered descriptors relevant to such information in a common ‘existence’ category. These are described in the table below.


| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_299  |  Document Creation Type |   This field is used to indicate the type of production activity used in the production of the described *Document*.   | Concept  |  --> P108i --> E12[58_1] --> P2 --> E55[299_1]|
|fie_cen_96 |   Document Creator  |  This field is used to record the actor who has created the documented *Document*.  |  Reference Model [Person/Group]|   --> P108i --> E12[58_1] --> P01i --> PC14[C96_1] --> P02 --> E39[C96_2]|
|fie_cen_97 |   Document Creator Role  |  This field is used to record the specific role of the actor they played in the creation of the documented *Document*.  |  Concept |   --> P108i --> E12[58_1] --> P01 --> PC14[C96_1] --> P14.1 --> E55[C97_1]|
|fie_cen_42 |   Document Creator Attribution |   This field is used to record the attribution type (renaissance or contemporary) assigning the creator of the described *Document*. |   Concept |   --> P108i --> E12[58_1]  --> P01i --> PC14[C96_1] --> P02 --> E39[C96_2] --> P141i --> E13[C42_1] --> P2 --> E55[C42_2]|
|fie_cen_43 |   Document Creator Source |   This field is used to relate a *Document* carrying a textual reference about the attribution assigning the creator of the described *Document* and the described *Document* itself. |   Reference Model [Document]|   --> P108i --> E12[58_1]  --> P01--> PC14[C96_1] --> P02 --> E39[C96_2] --> P141i --> E13[C42_1] -- >P16 --> E33[C43_1] --> P128i --> E22[C43_2]|
|fie_58 |   Document Creation Earliest Date |   This field is used to record the earliest possible date for the production of the described *Document*.   | Date |   --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P82a --> xsd:dateTime|
|fie_59 |   Document Creation Latest Date  |  This field is used to record the latest possible date for the production of the described *Document*.   | Date |   --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P82b --> xsd:dateTime|
|fie_61 |   Document Creation Period  |  This field is used to record the historical period in which the production of the described *Document* occurred. |   Reference Model [Period]|   --> P108i --> E12[58_1] --> P10 --> E4[61_1]|
|fie_cen_44  |  Document Creation Date Attribution  |  This field is used to record the attribution type (renaissance or contemporary) assigning the timespan of the production of the described *Document*.   | Concept |   --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P141i --> E13[C44_1] --> P2 --> E55[C44_2]|
|fie_cen_45  |  Document Creation Date Source  |  This field is used to relate a document carrying a textual reference about the attribution assigning timespan of the production of the described document and the described *Document* itself. |   Reference Model [Document]|   --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P141i --> E13[C44_1] --> P16 --> E33[C45_1] --> P128i --> E22[C45_2]|
|fie_cen_92 |   Document Creation Timespan Verbatim  |  This field is used to record a verbatim describing the timespan of the production event of the described *Document*.  |  String  |  --> P108i --> E12[58_1] --> P4 --> E52[58_2] --> P67i --> E33[C92_1] --> P190 --> rdfs:literal|
|fie_60  |  Document Creation Location |   This field is used to record the place of the production of the described *Document*.  |  Reference Model  [Place]|  --> P108i --> E12[58_1] --> P7 --> E53[60_1]|
|fie_cen_46 |   Document Creation Location Attribution  |  This field is used to record the attribution type (renaissance or contemporary) assigning the place of production of the described *Document*. |   Concept |   --> P108i --> E12[58_1] --> P7 --> E53[60_1] --> P141i --> E13[C46_1] --> P2 --> E55[C46_2]|
|fie_cen_47  |  Document Creation Location Source |   This field is used to relate a *Document* carrying a textual reference about the attribution assigning the place of production of the described *Document* and the described *Document* itself.  |  Reference Model  [Document]|  --> P108i --> E12[58_1] --> P7 --> E53[60_1] --> P141i --> E13[C46_1] --> P16 --> E33[C47_1] --> P128i --> E22[C47_2]|
|fie_cen_8  |  Document Destruction Type |   This field is used to record the generic type of the destruction event of the described *Document*. |   Concept |   --> P13i --> E6_E7[62_1] --> P2 --> E55[C8_1]|
|fie_cen_9 |   Document Destruction Actor |   This field is used to record an actor carried out the destruction event of the described *Document*.  |  Reference Model [Person/Group]|   --> P13i --> E6_E7[62_1] --> P01i --> PC14[C16_1] --> P02 --> E39[C9_1]|
|fie_cen_16 |   Document Destruction Actor Role |   This field is used to record the specific capacity in which an actor carried out the destruction event of the described *Document*. |   Concept  |  --> P13i --> E6_E7[62_1] --> P01 --> PC14[C16_1] --> P14.1 --> E55[C16_2]|
|fie_cen_17  |  Document Destruction Actor Attribution   | This field is used to record the attribution type (renaissance or contemporary) assigning an actor carried out he destruction event of the described *Document*. |   Concept |   --> P13i --> E6_E7[62_1] --> P01i --> PC14[C16_1] --> P02 --> E39[C9_1] -- P141i --> E13[C17_1] --> P2 --> E55[C17_2]|
|fie_cen_18 |   Document Destruction Actor Reference |   This field is used to relate a *Document* carrying a textual reference about the attribution (renaissance or contemporary) assigning an actor carried out he destruction event of the described *Document* and the described *Document* itself. |   Reference Model [Document]|   --> P13i --> E6_E7[62_1] --> P01i --> PC14[C16_1] --> P02 --> E39[C9_1] -- P141i --> E13[C17_1] -- >P16 --> E33[C18_1] --> P128i --> E22[C18_2]|
|fie_cen_7  |  Document Destruction Date |   This field is used to record the timespan of the destruction event of the described *Document*.  |  Collection [Timespan]|   --> P13i --> E6_E7[62_1]  --> P4 --> E52[62_2]|
|fie_cen_99   | Document Destruction Period  |  This field is used to record the period during which the destruction event of the documented *Document* has happened.  |  Reference Model [Period] |  --> P13i --> E6_E7[62_1] --> P10 --> E4 [C99_1]|

### - Document Existence **Ontology Graph**
![Screenshot](img/ex_document.png)

### - Document Existence **RDF**

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

<https://example.org/conceptual_object/C104_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C104_2> .

<https://example.org/conceptual_object/C18_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C18_2> .

<https://example.org/conceptual_object/C43_1> a crm:E33_Linguistic_Object ;
    crm:P128i_carried_by <https://example.org/physical_object/C43_2> .

<https://example.org/conceptual_object/C45_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C45_2> .

<https://example.org/conceptual_object/C47_1> a crm:E33_Linguistic_Object ;
    crm:P128i_is_carried_by <https://example.org/physical_object/C47_2> .

<https://example.org/conceptual_object/fie_92_1> a crm:E33_Linguistic_Object ;
    crm:P190_has_symbolic_content "timespan verbatim" .

<https://example.org/event/C103_1> a crm:E13_Attribute_Assignment ;
    crm:P16_used_specific_object <https://example.org/conceptual_object/C104_1> ;
    crm:P2_has_type <https://example.org/type/C103_2> .

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
    crm:P10_falls_within <https://example.org/period/C99_1> ;
    crm:P2_has_type <https://example.org/type/C8_1> ;
    crm:P4_has_time-span <https://example.org/time_span/fie_62_2> ;
    crm:P7_took_place_at <https://example.org/place/C102_1> .

<https://example.org/period/C99_1> a crm:E4_Period .

<https://example.org/physical_object/C104_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C18_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C43_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C45_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/C47_2> a crm:E22_Human-Made_Object .

<https://example.org/physical_object/fie_299_1> a crm:E55_Type .

<https://example.org/place/C102_1> a crm:E53_Place ;
    crm:P141i_was_assigned_by <https://example.org/event/C103_1> .

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
    crm:P67i_is_referred_to_by <https://example.org/conceptual_object/fie_92_1> ;
    crm:P82a_begin_of_the_begin ""^^xsd:dateTime ;
    crm:P82b_end_of_the_end ""^^xsd:dateTime .

<https://example.org/time_span/fie_62_2> a crm:E52_Time-Span .

<https://example.org/type/C103_2> a crm:E55_Type .

<https://example.org/type/C16_2> a crm:E55_Type .

<https://example.org/type/C17_2> a crm:E55_Type .

<https://example.org/type/C42_2> a crm:E55_Type .

<https://example.org/type/C44_2> a crm:E55_Type .

<https://example.org/type/C46_2> a crm:E55_Type .

<https://example.org/type/C8_1> a crm:E55_Type .

<https://example.org/type/C97_1> a crm:E55_Type .


```
                
### - Document Existence **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/physical_object/fie_299_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/physical_object/C43_2",
      "type": "HumanMadeObject"
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
      "id": "https://example.org/physical_object/C45_2",
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/period/C99_1",
      "type": "Period"
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
      "carried_by": [
        "https://example.org/physical_object/C104_2"
      ],
      "id": "https://example.org/conceptual_object/C104_1",
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
      "id": "https://example.org/physical_object/C104_2",
      "type": "HumanMadeObject"
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
      "assigned_by": [
        "https://example.org/event/C103_1"
      ],
      "id": "https://example.org/place/C102_1",
      "type": "Place"
    },
    {
      "carried_by": [
        "https://example.org/physical_object/C18_2"
      ],
      "id": "https://example.org/conceptual_object/C18_1",
      "type": "LinguisticObject"
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
      "id": "https://example.org/type/C17_2",
      "type": "Type"
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
      "id": "https://example.org/type/C103_2",
      "type": "Type"
    },
    {
      "assigned_by": [
        "https://example.org/event/C44_1"
      ],
      "begin_of_the_begin": "",
      "end_of_the_end": "",
      "id": "https://example.org/time_span/fie_58_2",
      "referred_to_by": [
        "https://example.org/conceptual_object/fie_92_1"
      ],
      "type": "TimeSpan"
    },
    {
      "id": "https://example.org/time_span/fie_62_2",
      "type": "TimeSpan"
    },
    {
      "classified_as": [
        "https://example.org/type/C103_2"
      ],
      "id": "https://example.org/event/C103_1",
      "type": "AttributeAssignment",
      "used_specific_object": [
        "https://example.org/conceptual_object/C104_1"
      ]
    },
    {
      "classified_as": [
        "https://example.org/type/C8_1"
      ],
      "crm:P01i_is_domain_of": {
        "id": "https://example.org/property/C16_1"
      },
      "falls_within": [
        "https://example.org/period/C99_1"
      ],
      "id": "https://example.org/event/fie_62_1",
      "timespan": "https://example.org/time_span/fie_62_2",
      "took_place_at": [
        "https://example.org/place/C102_1"
      ],
      "type": [
        "Destruction",
        "Activity"
      ]
    },
    {
      "content": "timespan verbatim",
      "id": "https://example.org/conceptual_object/fie_92_1",
      "type": "LinguisticObject"
    }
  ]
}
                
```

## Document **Events**
This information category brings together typical events in which a *Document* may have been involved through the course of its history. It is meant to cover information concerning the most salient events documented with regards to documents. At present this enables the documentation of provenance of the *Document*.

| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_269 |   Document Provenance Event Type  |  This field is used to indicate the type of a provenance activity associated with the documented *Document*.  |  Concept|    --> P16i --> E7[268_1] --> P2 --> E55[269_1]|
|fie_cen_98 |   Document Provenance Event Actor |   This field is used to record the actor participated in a provenance activity associated with the documented *Document*. |   Reference Model [Person/Group]|   --> P16i --> E7[268_1] --> P01i --> PC14[C70_1] --> P02 --> E39[C98_1]|
|fie_cen_70  |  Document Provenance Event Actor Role |   This field is used to indicate the specific role of the actor carried out the provenance activity associated with the documented *Document*. |   Concept  |  --> P16i --> E7[268_1] --> P01 --> PC14[C70_1] --> P14.1 --> E55[C70_2]|
|fie_cen_71  |  Document Provenance Event Actor Attribution  |  This field is used to record the type of attribution (renaissance or contemporary) assigning the actor carried out the provenance activity associated with the documented *Document*.  |  Concept |   --> P16i --> E7[268_1] --> P01 --> PC14[C70_1] --> P02 --> E39[C98_1] --> P141i -->E13[C71_1] --> P2 --> E55[C71_2]|
|fie_cen_72 |   Monument Provenance Event Actor Source  |  This field is used to record the *Document* carrying a textual reference about the type of attribution (Renaissance or contemporary) assigning the actor carried out the provenance activity associated with the documented *Monument* and the documented *Monument* itself. |   Reference Model [Document]|   --> P16i --> E7[268_1] --> P01 --> PC14[C70_1] --> P02 --> E39[C98_1] --> P141i -->E13[C71_1] --> P16 -->E33[C72_1] --> P128i -->E22[C72_2]|
|fie_cen_68 |   Document Provenance Event Timespan |   This field is used to record the timespan of a provenance activity associated with the documented *Document*. |   Collection  [Timespan]|  --> P16i --> E7[268_1] --> P4 --> E52[270_1] |
|fie_cen_73  |  Document Provenance Event Location  |  This field is used to record the location of the provenance activity associated with the documented *Document*. |   Reference Model [Location]|   --> P16i --> E7[268_1] --> P7 --> E53[C73_1]|
|fie_cen_75  |  Document Provenance Event Location Source |   This field is used to relate the *Document* carrying a textual reference about the type of attribution (Renaissance or contemporary) assigning the location of the provenance activity associated with the documented *Document* and the documented *Document* itself. |   Reference Model [Document]|   --> P16i --> E7[268_1] --> P7 --> E53[C73_1] --> P141i -->E13[C74_1] --> P16 -->E33[C75_1] --> P128i -->E22[C75_2]|
|fie_cen_74 |   Document Provenance Event Location Attribution |   This field is used to record the type of attribution (Renaissance or contemporary) assigning the location of the provenance activity associated with the documented *Document*.  |  Concept |   --> P16i --> E7[268_1] --> P7 --> E53[C73_1] --> P141i -->E13[C74_1] --> P2 --> E55[C74_2]|
|fie_cen_76 |   Document Provenance Event Statement |   This field is used to record a general statement about the provenance activity associated with the documented *Document*.   | Collection [Statement]|   --> P16i --> E7[268_1] --> P67i --> E33[C76_1]|
|fie_cen_100 |   Document Provenance Event Period |   This field is used to record the period during which a provenance activity associated with the documented *Document* has happened.  |  Reference Model [Period]|   --> P16i --> E7[268_1] --> P10 --> E4 [C100_1]|

### - Document Events **Ontology Graph**
![Screenshot](img/ev_document.png)

### - Document Events **RDF**
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
### - Document Events **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "classified_as": [
        "https://example.org/type/fie_17_1",
        "https://example.org/type/fie_201_1",
        "https://example.org/type/C56_1",
        "https://example.org/type/C21_1"
      ],
      "id": "https://census.de/example/physical_object/E22",
      "identified_by": [
        "https://example.org/name/fie_1_1",
        "https://example.org/name/fie_5_1",
        "https://example.org/name/fie_10_1"
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

## Document **Substance**
The analysis and understanding of a *Document* depends also on our knowledge of its materiality and physical characteristics. The category of substance brings together descriptors which are relevant to this form of analysis. Particularly, it groups information having to do with the composition and measurable aspects of the *Document* as an object, the physical carrier of the content, as well as the documentation of any inscriptions.
               
| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_90 |   Document Material|    This field is used to record the material of which the described document consists.  |  Concept   | --> P45 --> E57[90_1]|
|fie_86  |  Document Dimension Type  |  This field is used to record the type of dimension measured on the described *Document*.  |  Concept  |  --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P2 --> E55[86_3]|
|fie_cen_91  |  Document Dimension Verbatim |   This field is used to record a verbatim describing the dimensions of the documented described *Document*.  |  String|    --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P67i --> E33_41[C91_1] --> P190 --> rdfs:literal|
|fie_87 |   Document Dimension Value|    This field is used to record the value of the measured dimension of the described *Document*.|    Integer |   --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P90 --> xsd:decimal|
|fie_88   | Document Dimension Unit  |  This field is used to record the unit of the measured dimension of the described *Document*.   | Concept  |  --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P91 --> E58[88_1]|
|fie_89 |   Document Dimension Taker |   This field is used to record the actor who undertook the measurement producing the dimension of the described *Document*.  |  Reference Model [Person/Group]|   --> P39i --> E16[86_1] --> P14 --> E39[89_1]|
|fie_cen_55 |   Document Dimensions Comment |   This field is used to record the textual content of a statement made about the dimensions of the described *Document*.   | String |   --> P39i --> E16[86_1] --> P40 --> E54[86_2] --> P67i --> E33_41[C55_1] --> P190 --> rdfs:literal|
|fie_cen_26  |  Document Inscription Type |   This field is used to record the general type of inscription carried out by the *Document*. |   Concept |   --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> P2 --> E55[C26_1]|
|fie_cen_25  |  Document Inscription |   This field is used to record inscription carried out by the described *Document*.   | Reference Model [Bibliographic Entity]|   --> P128 --> E33[C22_1] --> P130 --> E33[C25_1]|
|fie_cen_28 |   Document Inscription Language |   This field is used to record the language of transcription carried out by the described *Document*. |   Concept |   --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> P72 --> E56[C28_1]|
|fie_cen_29  |  Document Inscription Name |   This field is used to record the formal name of the inscription carried out by the described *Document*. |   String  |  --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> P1 --> E33_E41[C29_1]|
|fie_cen_30 |   Document Inscription Reference |   This field is used to record the bibliographic reference of the inscription carried out by the described *Document*.|   Reference Model [Bibliographic Entity]|   --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> P67i --> E33[C30_1]|
|fie_cen_88  |  Document Inscription URL |   This field is used to record the external link of the linguistic object being in a similar or direct relationship with the linguistic object carried out by the described *Document*. |   URI  |  --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> L54 --> E1[88_1] |
|fie_cen_90  |  Document Inscription Position  |  This field is used to record a statement about the physical position of the linguistic object being in a similar or direct relationship with the linguistic object carried out by the described *Document*.  |  String  |  --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> P67i --> E33[C60_1] --> P190 --> rdfs:literal|
|fie_cen_27  |  Document Inscription Transcription|    This field is used to record the transcription of the inscription carried out by the described *Document*. |   String   | --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> P190 --> rdfs:literal|
|fie_cen_60    |Document Inscription Comments |   This field is used to record a general statement about the inscription carried out by the described *Document*. |   Collection  [Statement]|  --> P128 --> E33[C22_1] --> P130 --> E33[C25_1] --> P67i --> E33[C60_1]|

### - Document Substance **Ontology Graph**
![Screenshot](img/sub_document.png)

### - Document Substance **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P128_carries <https://example.org/conceptual_object/C22_1> ;
    crm:P39i_was_measured_by <https://example.org/event/fie_86_1> ;
    crm:P45_consists_of <https://example.org/type/material/fie_90_1> .

<https://example.org/actor/fie_89_1> a crm:E39_Actor .

<https://example.org/appellation/C29_1> a crm:E33_E41_Linguistic_Appellation .

<https://example.org/appellation/C55_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P190_has_symbolic_content "dimension statement" .

<https://example.org/appellation/C91_1> a crm:E33_E41_Linguistic_Appellation ;
    crm:P190_has_symbolic_content "dimension verbatim" .

<https://example.org/conceptual_object/C22_1> a crm:E33_Linguistic_Object ;
    crm:P130_shows_features_of <https://example.org/conceptual_object/C25_1> .

<https://example.org/conceptual_object/C25_1> a crm:E33_Linguistic_Object ;
    crm:L54_is_same-as <https://example.org/entity/C88_1> ;
    crm:P190_has_symbolic_content "transcription content" ;
    crm:P1_is_identified_by <https://example.org/appellation/C29_1> ;
    crm:P2_has_type <https://example.org/type/C26_1> ;
    crm:P67i_is_referred_by <https://example.org/conceptual_object/C30_1>,
        <https://example.org/conceptual_object/C60_1>,
        <https://example.org/conceptual_object/C90_1> ;
    crm:P72_has_language <https://example.org/type/C28_1> .

<https://example.org/conceptual_object/C30_1> a crm:E33_Linguistic_Object .

<https://example.org/conceptual_object/C60_1> a crm:E33_Linguistic_Object .

<https://example.org/conceptual_object/C90_1> a crm:E33_Linguistic_Object ;
    crm:P190_has_symbolic_content "position" .

<https://example.org/dimension/fie_86_2> a crm:E54_Dimension ;
    crm:P2_has_type <https://example.org/type/fie_86_3> ;
    crm:P67i_is_referred_by <https://example.org/appellation/C55_1>,
        <https://example.org/appellation/C91_1> ;
    crm:P90_has_value "content" ;
    crm:P91_has_unit <https://example.org/type/fie_88_1> .

<https://example.org/entity/C88_1> a crm:E1_CRM_Entity .

<https://example.org/event/fie_86_1> a crm:E16_Measurement ;
    crm:P14_carried_out_by <https://example.org/actor/fie_89_1> ;
    crm:P40_observed_dimension <https://example.org/dimension/fie_86_2> .

<https://example.org/type/C26_1> a crm:E55_Type .

<https://example.org/type/C28_1> a crm:E56_Language .

<https://example.org/type/fie_86_3> a crm:E55_Type .

<https://example.org/type/fie_88_1> a crm:E58_Measurement_Unit .

<https://example.org/type/material/fie_90_1> a crm:E57_Material .



                
```
### - Document Substance **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "classified_as": [
        "https://example.org/type/C26_1"
      ],
      "content": "transcription content",
      "crm:L54_is_same-as": {
        "id": "https://example.org/entity/C88_1"
      },
      "crm:P67i_is_referred_by": [
        {
          "id": "https://example.org/conceptual_object/C30_1"
        },
        {
          "id": "https://example.org/conceptual_object/C60_1"
        },
        {
          "id": "https://example.org/conceptual_object/C90_1"
        }
      ],
      "id": "https://example.org/conceptual_object/C25_1",
      "identified_by": [
        "https://example.org/appellation/C29_1"
      ],
      "language": [
        "https://example.org/type/C28_1"
      ],
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/conceptual_object/C22_1",
      "shows_features_of": [
        "https://example.org/conceptual_object/C25_1"
      ],
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/C26_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/actor/fie_89_1",
      "type": "Actor"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_86_3"
      ],
      "crm:P67i_is_referred_by": [
        {
          "id": "https://example.org/appellation/C91_1"
        },
        {
          "id": "https://example.org/appellation/C55_1"
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
      "carries": [
        "https://example.org/conceptual_object/C22_1"
      ],
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
      "id": "https://example.org/appellation/C29_1",
      "type": "Name"
    },
    {
      "id": "https://example.org/conceptual_object/C30_1",
      "type": "LinguisticObject"
    },
    {
      "carried_out_by": [
        "https://example.org/actor/fie_89_1"
      ],
      "id": "https://example.org/event/fie_86_1",
      "observed_dimension": [
        "https://example.org/dimension/fie_86_2"
      ],
      "type": "Measurement"
    },
    {
      "id": "https://example.org/type/material/fie_90_1",
      "type": "Material"
    },
    {
      "id": "https://example.org/conceptual_object/C60_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/type/fie_88_1",
      "type": "MeasurementUnit"
    },
    {
      "id": "https://example.org/type/C28_1",
      "type": "Language"
    },
    {
      "content": "position",
      "id": "https://example.org/conceptual_object/C90_1",
      "type": "LinguisticObject"
    },
    {
      "id": "https://example.org/entity/C88_1",
      "type": "CRMEntity"
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

## Document **Aboutness**
This information category provides the means to gather information to the representational level of a *Document*. 
               
| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_cen_23|    Document Medium Visual  |  This field is used to record the visual content carried out by the described *Document*.  |  Concept |   --> P65 --> E36[C23_1] --> P2 --> E55[C23_2]|
|fie_cen_22   | Document Medium Written  |  This field is used to record the type of textual content carried out by the described *Document*.  |  Concept  |  --> P128 --> E33[C22_1] --> P2 --> E55[C22_2]|


### - Document Aboutness **Ontology Graph**
![Screenshot](img/ab_document.png)

### - Document Aboutness **RDF**

```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:P128_carries <https://example.org/conceptual_object/C22_1> ;
    crm:P65_shows_visual_item <https://example.org/conceptual_object/C23_1> .

<https://example.org/conceptual_object/C22_1> a crm:E33_Linguistic_Object ;
    crm:P2_has_type <https://example.org/type/C22_2> .

<https://example.org/conceptual_object/C23_1> a crm:E36_Visual_Item ;
    crm:P2_has_type <https://example.org/type/C23_2> .

<https://example.org/type/C22_2> a crm:E55_Type .

<https://example.org/type/C23_2> a crm:E55_Type .


                
```
### - Document Aboutness **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "carries": [
        "https://example.org/conceptual_object/C22_1"
      ],
      "id": "https://census.de/example/physical_object/E22",
      "shows": [
        "https://example.org/conceptual_object/C23_1"
      ],
      "type": "HumanMadeObject"
    },
    {
      "id": "https://example.org/type/C23_2",
      "type": "Type"
    },
    {
      "id": "https://example.org/type/C22_2",
      "type": "Type"
    },
    {
      "classified_as": [
        "https://example.org/type/C22_2"
      ],
      "id": "https://example.org/conceptual_object/C22_1",
      "type": "LinguisticObject"
    },
    {
      "classified_as": [
        "https://example.org/type/C23_2"
      ],
      "id": "https://example.org/conceptual_object/C23_1",
      "type": "VisualItem"
    }
  ]
}
                
```


## Document **Location**
The documentation of location aids in tracking the present location of individual *Documents* as well their dispersion geographically. This information category gathers together relevant descriptors for this task.
               
| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_177 |  Document Location  |  This field is used to record the address at which the described *Document* is located.  |  String  |  --> P53 --> E53[177_1] --> P1 --> E41[177_2]<br><br>P53 --> E53[177_1] --> P1 --> E41[177_2] --> P2 --> E55 "Address"[177_3]|


### - Document Location **Ontology Graph**
![Screenshot](img/loc_document.png)
     
### - Document Location **RDF**
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

### - Document Location **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "_label": "Address",
      "id": "https://example.org/type/fie_177_3",
      "type": "Type"
    },
    {
      "former_or_current_location": [
        "https://example.org/place/fie_177_1"
      ],
      "id": "https://census.de/example/physical_object/E22",
      "type": "HumanMadeObject"
    },
    {
      "classified_as": [
        "https://example.org/type/fie_177_3"
      ],
      "id": "https://example.org/name/fie_177_2",
      "type": "Appellation"
    },
    {
      "id": "https://example.org/place/fie_177_1",
      "identified_by": [
        "https://example.org/name/fie_177_2"
      ],
      "type": "Place"
    }
  ]
}
                
```           

## Document **Description**
Documents are the subjects of innumerable descriptions that provide a wide range of information with regards to the aesthetic and historical importance of the work, inter alia. Such descriptions are of use in a scholarly understanding of a *Document* just in case we are able to track the provenance of such elocutions in a systematic fashion. Such an aim drives the need for the tracking of description information as a separate category. The descriptors necessary to this task are documented in the table below.

               
| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_cen_32 |   Document Relation Type |   This field is used to record the type of similarity between the described *Document* and another *Document*. |   Concept   | --> P01i --> PC130[C31_1] --> P130.1 --> E55[C32_1]|
|fie_cen_31 |   Document Relation |   This field is used to record the type of similarity between the described *Document* and another *Document*.  |  Reference Model  [Document]|  --> P01i --> PC130[C31_1] --> P02 --> E22[C31_2] |
|fie_cen_58  |  Document Notes|    This field is used to record a general statement about the described *Document*.   | Collection [Statement] |  --> P67i --> E33[C58_1]|

### - Document Description **Ontology Graph**
![Screenshot](img/desc_document.png)
     
### - Document Description **RDF**
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

### - Document Description **JSON-LD**
```
{
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/physical_object/C31_2",
      "type": "crm:E22_Human-made_Object"
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
    }
  ]
}
                
```
## Document **Documentation**
This information category unites referential information about the documented *Document*, providing contextual data about it.
               
| Filed ID    | Name                          | Description | Data Type | CRM Path |
| ----------- | ------------------------------|-------------|-----------|----------|
|fie_196  |  Document Citation  |  This field is used to record a citation to reference documentation for the described *Document*.  |  String  |  --> P129i --> E33[196_1] --> rdf:value --> rdfs:Literal<br><br>--> P129i --> E33[196_1] --> P2 --> E55 "Citation" |
|fie_197  |  Document Citation Source  |  This field is used to record the source used for generating the citation for the described *Document*.  |  Reference Model [Bibliographic Entity]|  --> P129i --> E33[196_1] --> P106i --> E33[197_1]|
|fie_cen_13  |  Document Bibliography |   This field is used to record a bibliographic reference for the described *Document*.  |  Reference Model  [Bibliographic Entity]|  --> P67i -->E33[C13_1]|
|fie_195  |  Document Image  |  This field is used to record a digital image which is representative of the described *Document*.  |  Reference Model [Image]|   --> P138i --> E36/D9[195_1]|
|fie_204   | Document URL  |  The field is used to record the sameness between the described *Document* and an external authority|    uri  |  --> L54 --> E1[204_1]|
|fie_cen_57 |   Document URL Title  |  The field is used to record the sameness between the described *Document* and an external authority.  |  String  |  --> L54 --> E1[204_1] --> P1 --> E33_E41[C57_1]|

### - Document Documentation **Ontology Graph**
![Screenshot](img/doc_document.png)
     
### - Document Documentation **RDF**
```
@prefix crm: <http://www.cidoc-crm.org/cidoc-crm/> .
@prefix rdfs: <http://www.w3.org/2000/01/rdf-schema#> .

<https://census.de/example/physical_object/E22> a crm:E22_Human-Made_Object ;
    crm:L54_is_same-as <https://example.org/entity/fie_204_1> ;
    crm:P129i_is_subject_of <https://example.org/conceptual_object/fie_196_1> ;
    crm:P138i_has_representation <https://example.org/conceptual_object/fie_195_1> ;
    crm:P67i_is_referred_to_by <https://example.org/conceptual_object/C13_1> .

<https://example.org/appellation/C57_1> a crm:E33_E41_Linguistic_Appellation .

<https://example.org/conceptual_object/C13_1> a crm:E33_Linguistic_Object .

<https://example.org/conceptual_object/fie_195_1> a crm:D9_Data_Object,
        crm:E36_Visual_Item .

<https://example.org/conceptual_object/fie_196_1> a crm:E33_Linguistic_Object ;
    crm:P106i_forms_part_of <https://example.org/conceptual_object/fie_197_1> ;
    crm:P190_has_symbolic_content "content" ;
    crm:P2_has_type <https://example.org/type/fie_196_1> .

<https://example.org/conceptual_object/fie_197_1> a crm:E33_Linguistic_Object .

<https://example.org/entity/fie_204_1> a crm:E1_CRM_Entity ;
    crm:P1_is_identified_by <https://example.org/appellation/C57_1> .

<https://example.org/type/fie_196_1> a crm:E55_Type ;
    rdfs:label "Citation" .
```

### - Document Documentation **JSON-LD**
```
    {
  "@context": "https://linked.art/ns/v1/linked-art.json",
  "@graph": [
    {
      "id": "https://example.org/conceptual_object/C13_1",
      "type": "LinguisticObject"
    },
    {
      "crm:L54_is_same-as": {
        "id": "https://example.org/entity/fie_204_1"
      },
      "id": "https://census.de/example/physical_object/E22",
      "referred_to_by": [
        "https://example.org/conceptual_object/C13_1"
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
      "id": "https://example.org/entity/fie_204_1",
      "identified_by": [
        "https://example.org/appellation/C57_1"
      ],
      "type": "CRMEntity"
    },
    {
      "id": "https://example.org/conceptual_object/fie_197_1",
      "type": "LinguisticObject"
    },
    {
      "_label": "Citation",
      "id": "https://example.org/type/fie_196_1",
      "type": "Type"
    },
    {
      "id": "https://example.org/conceptual_object/fie_195_1",
      "type": [
        "VisualItem",
        "crm:D9_Data_Object"
      ]
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
      "id": "https://example.org/appellation/C57_1",
      "type": "Name"
    }
  ]
}
```                            
