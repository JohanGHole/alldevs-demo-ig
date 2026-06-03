# HIV Follow-up Reasons - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV Follow-up Reasons 

 
Reasons for HIV follow-up. 

This Code system is referenced in the definition of the following value sets:

* [HIVReasonsForFollowUpVS](ValueSet-HIVReasonsForFollowUpVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVReasonsForFollowUp",
  "url" : "https://dhis2.org/CodeSystem/HIVReasonsForFollowUp",
  "version" : "1.0.0",
  "name" : "HIVReasonsForFollowUp",
  "title" : "HIV Follow-up Reasons",
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
  "description" : "Reasons for HIV follow-up.",
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
    "code" : "MISSED_CLINICAL_VISIT",
    "display" : "Missed clinical care visit"
  },
  {
    "code" : "MISSED_ARV_PICKUP",
    "display" : "Missed medication pickup"
  },
  {
    "code" : "MISSED_VISIT_NONCLINICAL",
    "display" : "Missed non-clinical visit"
  },
  {
    "code" : "ART_NOT_STARTED",
    "display" : "Did not initiate ART"
  },
  {
    "code" : "HIV_INCONCLUSIVE",
    "display" : "Inconclusive HIV status"
  },
  {
    "code" : "TEST_RESULTS",
    "display" : "Test results received"
  },
  {
    "code" : "OTHER_REASON",
    "display" : "Other follow up reason (specify)"
  }]
}

```
