# DHIS2 Metadata: AttributeValue - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: DHIS2 Metadata: AttributeValue 

 
DHIS2 Metadata: AttributeValue 

**Usages:**

* Use this Logical Model: [DHIS2 Metadata: OptionSet](StructureDefinition-d2-md-option-set.md), [DHIS2 Metadata: Option](StructureDefinition-d2-md-option.md) and [DHIS2 Metadata: OrganisationUnit](StructureDefinition-d2-md-organisation-unit.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-d2-md-attribute-value.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-d2-md-attribute-value.csv), [Excel](../StructureDefinition-d2-md-attribute-value.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "d2-md-attribute-value",
  "url" : "https://dhis2.org/StructureDefinition/d2-md-attribute-value",
  "version" : "1.0.0",
  "name" : "MDAttributeValue",
  "title" : "DHIS2 Metadata: AttributeValue",
  "status" : "draft",
  "date" : "2026-06-03T19:24:40+00:00",
  "publisher" : "DHIS2",
  "contact" : [{
    "name" : "DHIS2",
    "telecom" : [{
      "system" : "url",
      "value" : "https://dhis2.org"
    },
    {
      "system" : "email",
      "value" : "integration@dhis2.org"
    }]
  },
  {
    "name" : "Johan Hole",
    "telecom" : [{
      "system" : "email",
      "value" : "Johan@Devotta.no",
      "use" : "work"
    }]
  }],
  "description" : "DHIS2 Metadata: AttributeValue",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "kind" : "logical",
  "abstract" : false,
  "type" : "https://dhis2.org/StructureDefinition/d2-md-attribute-value",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "d2-md-attribute-value",
      "path" : "d2-md-attribute-value",
      "short" : "DHIS2 Metadata: AttributeValue",
      "definition" : "DHIS2 Metadata: AttributeValue"
    },
    {
      "id" : "d2-md-attribute-value.attribute",
      "path" : "d2-md-attribute-value.attribute",
      "short" : "Attribute UID",
      "definition" : "Attribute UID",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-attribute-value.value",
      "path" : "d2-md-attribute-value.value",
      "short" : "Value of attribute",
      "definition" : "Value of attribute",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    }]
  }
}

```
