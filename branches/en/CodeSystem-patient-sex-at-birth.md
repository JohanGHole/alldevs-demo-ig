# Patient Sex at Birth - DHIS2 Example FHIR Implementation Guide v1.0.0

## CodeSystem: Patient Sex at Birth 

 
Patient sex at birth. 

This Code system is referenced in the definition of the following value sets:

* [PatientSexAtBirthVS](ValueSet-patient-sex-at-birth-vs.md)

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "CodeSystem",
  "id" : "patient-sex-at-birth",
  "url" : "https://dhis2.org/CodeSystem/patient-sex-at-birth",
  "version" : "1.0.0",
  "name" : "PatientSexAtBirth",
  "title" : "Patient Sex at Birth",
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
  "description" : "Patient sex at birth.",
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
    "code" : "male",
    "display" : "Male",
    "designation" : [{
      "language" : "pt",
      "value" : "Masculino"
    },
    {
      "language" : "es",
      "value" : "Masculino"
    },
    {
      "language" : "et",
      "value" : "Mees"
    }]
  },
  {
    "code" : "female",
    "display" : "Female",
    "designation" : [{
      "language" : "pt",
      "value" : "Feminino"
    },
    {
      "language" : "es",
      "value" : "Feminino"
    },
    {
      "language" : "et",
      "value" : "Naine"
    }]
  },
  {
    "code" : "other",
    "display" : "Other",
    "designation" : [{
      "language" : "pt",
      "value" : "Outro"
    },
    {
      "language" : "es",
      "value" : "Otro"
    },
    {
      "language" : "et",
      "value" : "Muu"
    }]
  },
  {
    "code" : "unknown",
    "display" : "Unknown",
    "designation" : [{
      "language" : "pt",
      "value" : "Desconhecido"
    },
    {
      "language" : "es",
      "value" : "Desconocido"
    },
    {
      "language" : "et",
      "value" : "Teadmata"
    }]
  }]
}

```
