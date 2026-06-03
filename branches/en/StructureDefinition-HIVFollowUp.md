# HIV Follow-Up - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: HIV Follow-Up 

 
Report filled out for follow-up. 

**Usages:**

* Use this Logical Model: [HIV Case Surveillance](StructureDefinition-HIVView.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-HIVFollowUp.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-HIVFollowUp.csv), [Excel](../StructureDefinition-HIVFollowUp.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "HIVFollowUp",
  "url" : "https://dhis2.org/StructureDefinition/HIVFollowUp",
  "version" : "1.0.0",
  "name" : "HIVFollowUp",
  "title" : "HIV Follow-Up",
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
  "description" : "Report filled out for follow-up.",
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
  "type" : "https://dhis2.org/StructureDefinition/HIVFollowUp",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "HIVFollowUp",
      "path" : "HIVFollowUp",
      "short" : "HIV Follow-Up",
      "definition" : "Report filled out for follow-up."
    },
    {
      "id" : "HIVFollowUp.followUpAttemptDate",
      "path" : "HIVFollowUp.followUpAttemptDate",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "date"
      }]
    },
    {
      "id" : "HIVFollowUp.followUpMethod",
      "path" : "HIVFollowUp.followUpMethod",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Coding"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "https://dhis2.org/ValueSet/HIVFollowUpMethodsVS"
      }
    },
    {
      "id" : "HIVFollowUp.followUpOutcome",
      "path" : "HIVFollowUp.followUpOutcome",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Coding"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "https://dhis2.org/ValueSet/HIVFollowUpOutcomesVS"
      }
    },
    {
      "id" : "HIVFollowUp.followUpReason",
      "path" : "HIVFollowUp.followUpReason",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Coding"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "https://dhis2.org/ValueSet/HIVReasonsForFollowUpVS"
      }
    },
    {
      "id" : "HIVFollowUp.followUpNotes",
      "path" : "HIVFollowUp.followUpNotes",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    }]
  }
}

```
