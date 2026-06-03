# HIV Follow-up Methods - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV Follow-up Methods 

 
Methods used for HIV follow-up. 

This Code system is referenced in the definition of the following value sets:

* [HIVFollowUpMethodsVS](ValueSet-HIVFollowUpMethodsVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVFollowUpMethods",
  "url" : "https://dhis2.org/CodeSystem/HIVFollowUpMethods",
  "version" : "1.0.0",
  "name" : "HIVFollowUpMethods",
  "title" : "HIV Follow-up Methods",
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
  "description" : "Methods used for HIV follow-up.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "content" : "complete",
  "count" : 4,
  "concept" : [{
    "code" : "SMS",
    "display" : "Text message"
  },
  {
    "code" : "PHONECALL",
    "display" : "Phone"
  },
  {
    "code" : "HOMEVISIT",
    "display" : "Home Visit"
  },
  {
    "code" : "OTHER",
    "display" : "Other"
  }]
}

```
