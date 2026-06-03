# HIV Follow-up Outcomes - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV Follow-up Outcomes 

 
Outcomes for HIV follow-up. 

This Code system is referenced in the definition of the following value sets:

* [HIVFollowUpOutcomesVS](ValueSet-HIVFollowUpOutcomesVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVFollowUpOutcomes",
  "url" : "https://dhis2.org/CodeSystem/HIVFollowUpOutcomes",
  "version" : "1.0.0",
  "name" : "HIVFollowUpOutcomes",
  "title" : "HIV Follow-up Outcomes",
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
  "description" : "Outcomes for HIV follow-up.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "content" : "complete",
  "count" : 7,
  "concept" : [{
    "code" : "RESCHEDULED",
    "display" : "Returning to clinic"
  },
  {
    "code" : "TRANSFERRED_OUT",
    "display" : "Self-transferred out"
  },
  {
    "code" : "HOSPITALIZED",
    "display" : "Hospitalized"
  },
  {
    "code" : "REFUSED_TO_RETURN",
    "display" : "Refused to return"
  },
  {
    "code" : "NORESPONSE",
    "display" : "Not located"
  },
  {
    "code" : "DIED_REPORTED",
    "display" : "Died (reported)"
  },
  {
    "code" : "DIED_CONFIRMED",
    "display" : "Confirmed Dead"
  }]
}

```
