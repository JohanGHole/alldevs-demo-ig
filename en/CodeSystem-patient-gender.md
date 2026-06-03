# Patient Gender - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: Patient Gender 

 
Patient gender codes. 

This Code system is referenced in the definition of the following value sets:

* [HIVPatientGenderVS](ValueSet-HIVPatientGenderVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "patient-gender",
  "url" : "https://dhis2.org/CodeSystem/patient-gender",
  "version" : "1.0.0",
  "name" : "HIVPatientGender",
  "title" : "Patient Gender",
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
  "description" : "Patient gender codes.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "content" : "complete",
  "count" : 5,
  "concept" : [{
    "code" : "male",
    "display" : "Male"
  },
  {
    "code" : "female",
    "display" : "Female"
  },
  {
    "code" : "transgender",
    "display" : "Transgender"
  },
  {
    "code" : "other",
    "display" : "Other"
  },
  {
    "code" : "unknown",
    "display" : "Unknown"
  }]
}

```
