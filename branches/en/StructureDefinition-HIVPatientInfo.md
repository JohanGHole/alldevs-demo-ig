# HIV Patient Data Model - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: HIV Patient Data Model 

 
Extension of the base patient data model. Includes properties specific to the HIV program. 

**Usages:**

* Use this Logical Model: [HIV Case Surveillance](StructureDefinition-HIVView.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-HIVPatientInfo.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-HIVPatientInfo.csv), [Excel](../StructureDefinition-HIVPatientInfo.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "HIVPatientInfo",
  "url" : "https://dhis2.org/StructureDefinition/HIVPatientInfo",
  "version" : "1.0.0",
  "name" : "HIVPatientInfo",
  "title" : "HIV Patient Data Model",
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
  "description" : "Extension of the base patient data model. Includes properties specific to the HIV program.",
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
  "type" : "https://dhis2.org/StructureDefinition/HIVPatientInfo",
  "baseDefinition" : "https://dhis2.org/StructureDefinition/PatientInfo",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "HIVPatientInfo",
      "path" : "HIVPatientInfo",
      "short" : "HIV Patient Data Model",
      "definition" : "Extension of the base patient data model. Includes properties specific to the HIV program."
    },
    {
      "id" : "HIVPatientInfo.hivEnrollmentUnit",
      "path" : "HIVPatientInfo.hivEnrollmentUnit",
      "short" : "The organization unit that first registered the person.",
      "definition" : "The organization unit that first registered the person.",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "HIVPatientInfo.programNationaId",
      "path" : "HIVPatientInfo.programNationaId",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "HIVPatientInfo.deceased",
      "path" : "HIVPatientInfo.deceased",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVPatientInfo.deceasedDate",
      "path" : "HIVPatientInfo.deceasedDate",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVPatientInfo.gender",
      "path" : "HIVPatientInfo.gender",
      "comment" : "(valueset depends on the program)",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Coding"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "https://dhis2.org/ValueSet/HIVPatientGenderVS"
      }
    },
    {
      "id" : "HIVPatientInfo.healthFacilityCode",
      "path" : "HIVPatientInfo.healthFacilityCode",
      "short" : "Health facility code.",
      "definition" : "Health facility code.",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "HIVPatientInfo.nhisId",
      "path" : "HIVPatientInfo.nhisId",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    }]
  }
}

```
