# HIV Reasons for Visit - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV Reasons for Visit 

 
HIV reasons for visit. 

This Code system is referenced in the definition of the following value sets:

* [HIVreasonsForVisitVS](ValueSet-HIVreasonsForVisitVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVreasonsForVisit",
  "url" : "https://dhis2.org/CodeSystem/HIVreasonsForVisit",
  "version" : "1.0.0",
  "name" : "HIVreasonsForVisit",
  "title" : "HIV Reasons for Visit",
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
  "description" : "HIV reasons for visit.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "content" : "complete",
  "count" : 3,
  "concept" : [{
    "code" : "CLINICAL_VISIT",
    "display" : "Clinical visit"
  },
  {
    "code" : "ARV_PICKUP",
    "display" : "Antiretroviral drug pick up"
  },
  {
    "code" : "ISSUES",
    "display" : "Issues and concerns"
  }]
}

```
