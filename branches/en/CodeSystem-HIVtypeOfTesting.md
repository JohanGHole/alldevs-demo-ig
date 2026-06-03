# HIV Type of Testing - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV Type of Testing 

 
HIV type of community-level testing. 

This Code system is referenced in the definition of the following value sets:

* [HIVtypeOfTestingVS](ValueSet-HIVtypeOfTestingVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVtypeOfTesting",
  "url" : "https://dhis2.org/CodeSystem/HIVtypeOfTesting",
  "version" : "1.0.0",
  "name" : "HIVtypeOfTesting",
  "title" : "HIV Type of Testing",
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
  "description" : "HIV type of community-level testing.",
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
    "code" : "MOBILE",
    "display" : "Mobile testing (e.g. through vans or temporary testing facilities)"
  },
  {
    "code" : "VOLUNTARYCTC",
    "display" : "Voluntary counceling and testing centres (not within a health facility setting)"
  },
  {
    "code" : "OTHERCOMMUNITY",
    "display" : "Other community based testing"
  }]
}

```
