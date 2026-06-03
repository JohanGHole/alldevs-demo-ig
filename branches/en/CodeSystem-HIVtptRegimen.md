# HIV TPT Regimen - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: HIV TPT Regimen 

 
HIV TPT regimen. 

This Code system is referenced in the definition of the following value sets:

* [HIVtptRegimenVS](ValueSet-HIVtptRegimenVS.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "HIVtptRegimen",
  "url" : "https://dhis2.org/CodeSystem/HIVtptRegimen",
  "version" : "1.0.0",
  "name" : "HIVtptRegimen",
  "title" : "HIV TPT Regimen",
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
  "description" : "HIV TPT regimen.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "content" : "complete",
  "count" : 8,
  "concept" : [{
    "code" : "1HP",
    "display" : "1HP (one month of daily rifapentine plus isoniazid)"
  },
  {
    "code" : "3HP",
    "display" : "3HP (three months of weekly rifapentine plus isoniazid)"
  },
  {
    "code" : "3RH",
    "display" : "3RH (three months of daily rifampicin plus isoniazid)"
  },
  {
    "code" : "4R",
    "display" : "4R (four months of daily rifampicin monotherapy)"
  },
  {
    "code" : "6H",
    "display" : "6H (six months of daily isoniazid monotherapy)"
  },
  {
    "code" : "9H",
    "display" : "9H (nine months of daily isoniazid monotherapy)"
  },
  {
    "code" : "INH-B6",
    "display" : "Combination INH-B6-Cotrim (for the duration of INH specified)"
  },
  {
    "code" : "OTHERTPT",
    "display" : "Other"
  }]
}

```
