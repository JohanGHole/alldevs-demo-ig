# DHIS2 Metadata: OptionSet - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: DHIS2 Metadata: OptionSet 

 
DHIS2 Metadata: OptionSet 

**Usages:**

* This Logical Model is not used by any profiles in this Specification

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-d2-md-option-set.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-d2-md-option-set.csv), [Excel](../StructureDefinition-d2-md-option-set.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "d2-md-option-set",
  "url" : "https://dhis2.org/StructureDefinition/d2-md-option-set",
  "version" : "1.0.0",
  "name" : "MDOptionSet",
  "title" : "DHIS2 Metadata: OptionSet",
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
  "description" : "DHIS2 Metadata: OptionSet",
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
  "type" : "https://dhis2.org/StructureDefinition/d2-md-option-set",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "d2-md-option-set",
      "path" : "d2-md-option-set",
      "short" : "DHIS2 Metadata: OptionSet",
      "definition" : "DHIS2 Metadata: OptionSet"
    },
    {
      "id" : "d2-md-option-set.id",
      "path" : "d2-md-option-set.id",
      "short" : "Unique UID for option set",
      "definition" : "Unique UID for option set",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-option-set.code",
      "path" : "d2-md-option-set.code",
      "short" : "Unique CODE for option set",
      "definition" : "Unique CODE for option set",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-option-set.href",
      "path" : "d2-md-option-set.href",
      "short" : "Unique URL where the option set is available from",
      "definition" : "Unique URL where the option set is available from",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-option-set.name",
      "path" : "d2-md-option-set.name",
      "short" : "Name of option set",
      "definition" : "Name of option set",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-option-set.shortName",
      "path" : "d2-md-option-set.shortName",
      "short" : "Short name of option set",
      "definition" : "Short name of option set",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-option-set.description",
      "path" : "d2-md-option-set.description",
      "short" : "Description of option set",
      "definition" : "Description of option set",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-option-set.options",
      "path" : "d2-md-option-set.options",
      "short" : "programs associated with this option set",
      "definition" : "programs associated with this option set",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "https://dhis2.org/StructureDefinition/d2-md-option"
      }]
    },
    {
      "id" : "d2-md-option-set.attributeValues",
      "path" : "d2-md-option-set.attributeValues",
      "short" : "additional attributes that are in this option set",
      "definition" : "additional attributes that are in this option set",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "https://dhis2.org/StructureDefinition/d2-md-attribute-value"
      }]
    }]
  }
}

```
