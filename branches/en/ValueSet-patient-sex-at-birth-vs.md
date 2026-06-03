# Patient Sex at Birth Value Set - DHIS2 Example FHIR Implementation Guide v1.0.0

## ValueSet: Patient Sex at Birth Value Set 

 
patient sex at birth value set. 

 **References** 

* [Base Patient Data Model](StructureDefinition-PatientInfo.md)

### Logical Definition (CLD)

 

### Expansion

-------

 [Description of the above table(s)](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#terminology). 



## Resource Content

```json
{
  "resourceType" : "ValueSet",
  "id" : "patient-sex-at-birth-vs",
  "url" : "https://dhis2.org/ValueSet/patient-sex-at-birth-vs",
  "version" : "1.0.0",
  "name" : "PatientSexAtBirthVS",
  "title" : "Patient Sex at Birth Value Set",
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
  "description" : "patient sex at birth value set.",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "compose" : {
    "include" : [{
      "system" : "https://dhis2.org/CodeSystem/patient-sex-at-birth"
    }]
  }
}

```
