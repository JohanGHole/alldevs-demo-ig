# HIV Treatment Status - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV Treatment Status 

 
HIV treatment status. 

This Code system is referenced in the definition of the following value sets:

* [HIVtreatmentStatusVS](ValueSet-HIVtreatmentStatusVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVtreatmentStatus",
  "url" : "https://dhis2.org/CodeSystem/HIVtreatmentStatus",
  "version" : "1.0.0",
  "name" : "HIVtreatmentStatus",
  "title" : "HIV Treatment Status",
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
  "description" : "HIV treatment status.",
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
    "code" : "RETAINED",
    "display" : "On ART"
  },
  {
    "code" : "DEAD",
    "display" : "Death (documented)"
  },
  {
    "code" : "TREATMENTSTOPPED",
    "display" : "Refused (stopped) treatment"
  },
  {
    "code" : "TRANSFEROUT",
    "display" : "Transferred out"
  },
  {
    "code" : "LTFU",
    "display" : "Lost to follow up"
  }]
}

```
