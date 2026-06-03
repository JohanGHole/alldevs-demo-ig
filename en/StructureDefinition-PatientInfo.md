# Base Patient Data Model - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: Base Patient Data Model 

 
Representation of common DHIS2 tracked entity properties. 

**Usages:**

* Derived from this Logical Model: [HIV Patient Data Model](StructureDefinition-HIVPatientInfo.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-PatientInfo.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-PatientInfo.csv), [Excel](../StructureDefinition-PatientInfo.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "PatientInfo",
  "url" : "https://dhis2.org/StructureDefinition/PatientInfo",
  "version" : "1.0.0",
  "name" : "PatientInfo",
  "title" : "Base Patient Data Model",
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
  "description" : "Representation of common DHIS2 tracked entity properties.",
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
  "type" : "https://dhis2.org/StructureDefinition/PatientInfo",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "PatientInfo",
      "path" : "PatientInfo",
      "short" : "Base Patient Data Model",
      "definition" : "Representation of common DHIS2 tracked entity properties."
    },
    {
      "id" : "PatientInfo.registrationDateTime",
      "path" : "PatientInfo.registrationDateTime",
      "short" : "Date-Time information was entered",
      "definition" : "Date and Time when the patient information was entered into DHIS2",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "dateTime"
      }]
    },
    {
      "id" : "PatientInfo.firstregisteredAt",
      "path" : "PatientInfo.firstregisteredAt",
      "short" : "The Org unit where the patient was first registered",
      "definition" : "The Org unit where the patient was first registered",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["http://hl7.org/fhir/StructureDefinition/Organization"]
      }]
    },
    {
      "id" : "PatientInfo.firstName",
      "path" : "PatientInfo.firstName",
      "short" : "Given name of the patient",
      "definition" : "Given name of the patient",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "PatientInfo.lastName",
      "path" : "PatientInfo.lastName",
      "short" : "Family name",
      "definition" : "Family name",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "PatientInfo.dateOfBirth",
      "path" : "PatientInfo.dateOfBirth",
      "short" : "...",
      "definition" : "...",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "PatientInfo.dateOfBirthIsEstimated",
      "path" : "PatientInfo.dateOfBirthIsEstimated",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "PatientInfo.sexAtBirth",
      "path" : "PatientInfo.sexAtBirth",
      "short" : "...",
      "definition" : "...",
      "comment" : "(valueset depends on the program)",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "code"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "https://dhis2.org/ValueSet/patient-sex-at-birth-vs"
      }
    },
    {
      "id" : "PatientInfo.currentHomeAddress",
      "path" : "PatientInfo.currentHomeAddress",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "PatientInfo.contactPhoneNumber",
      "path" : "PatientInfo.contactPhoneNumber",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "PatientInfo.countryOfBirth",
      "path" : "PatientInfo.countryOfBirth",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "urn:iso:std:iso:3166"
      }
    },
    {
      "id" : "PatientInfo.nationaId",
      "path" : "PatientInfo.nationaId",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "PatientInfo.consent",
      "path" : "PatientInfo.consent",
      "short" : "...",
      "definition" : "...",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    }]
  }
}

```
