# HIV Case Surveillance - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: HIV Case Surveillance 

 
Logical model representation of the HIV case surveillance and treatment follow up program. 

**Usages:**

* This Logical Model is not used by any profiles in this Specification

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-HIVView.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-HIVView.csv), [Excel](../StructureDefinition-HIVView.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "HIVView",
  "url" : "https://dhis2.org/StructureDefinition/HIVView",
  "version" : "1.0.0",
  "name" : "HIVView",
  "title" : "HIV Case Surveillance",
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
  "description" : "Logical model representation of the HIV case surveillance and treatment follow up program.",
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
  "type" : "https://dhis2.org/StructureDefinition/HIVView",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "HIVView",
      "path" : "HIVView",
      "short" : "HIV Case Surveillance",
      "definition" : "Logical model representation of the HIV case surveillance and treatment follow up program."
    },
    {
      "id" : "HIVView.caseReport",
      "path" : "HIVView.caseReport",
      "short" : "HIV Initial Case Report",
      "definition" : "HIV Initial Case Report",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "https://dhis2.org/StructureDefinition/HIVCaseData"
      }]
    },
    {
      "id" : "HIVView.visit",
      "path" : "HIVView.visit",
      "short" : "HIV Visit",
      "definition" : "HIV Visit",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "https://dhis2.org/StructureDefinition/HIVCaseVisitData"
      }]
    },
    {
      "id" : "HIVView.followUp",
      "path" : "HIVView.followUp",
      "short" : "HIV Follow-Up",
      "definition" : "HIV Follow-Up",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "https://dhis2.org/StructureDefinition/HIVFollowUp"
      }]
    },
    {
      "id" : "HIVView.patient",
      "path" : "HIVView.patient",
      "short" : "HIV Patient Info",
      "definition" : "HIV Patient Info",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "https://dhis2.org/StructureDefinition/HIVPatientInfo"
      }]
    }]
  }
}

```
