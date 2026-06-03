# HIV Entry Points for Facility-Level Testing - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV Entry Points for Facility-Level Testing 

 
HIV entry points for facility-level testing. 

This Code system is referenced in the definition of the following value sets:

* [HIVfacilityLevelTestingEntryPointsVS](ValueSet-HIVfacilityLevelTestingEntryPointsVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVfacilityLevelTestingEntryPoints",
  "url" : "https://dhis2.org/CodeSystem/HIVfacilityLevelTestingEntryPoints",
  "version" : "1.0.0",
  "name" : "HIVfacilityLevelTestingEntryPoints",
  "title" : "HIV Entry Points for Facility-Level Testing",
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
  "description" : "HIV entry points for facility-level testing.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "content" : "complete",
  "count" : 6,
  "concept" : [{
    "code" : "PROVIDERINITIATED",
    "display" : "Provider-initiated tested in a clinic or emergency facility"
  },
  {
    "code" : "ANTENATALCLINIC",
    "display" : "Antenatal care clinic"
  },
  {
    "code" : "VOLUNTARYCOUNSELLING",
    "display" : "Voluntary Counselling and Testing (within a health facility setting)"
  },
  {
    "code" : "FAMILYPLANNING",
    "display" : "Family planning clinic"
  },
  {
    "code" : "OTHERFACILITY",
    "display" : "Other facility-level testing"
  },
  {
    "code" : "TBCLINIC",
    "display" : "TB clinic"
  }]
}

```
