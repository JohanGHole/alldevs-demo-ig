# MDOrganisationUnitOrganization-Sierra-Leone - DHIS2 Example FHIR Implementation Guide v1.0.0

## Example Organization: MDOrganisationUnitOrganization-Sierra-Leone

Profile: [MDOrganisationUnit Organization](StructureDefinition-MDOrganisationUnitOrganization.md)

**Organization Period**: 1994-01-01 --> (ongoing)

**identifier**: id/ImspTQPwCqd, code/OU_525

**name**: Sierra Leone



## Resource Content

```json
{
  "resourceType" : "Organization",
  "id" : "MDOrganisationUnitOrganization-Sierra-Leone",
  "meta" : {
    "profile" : ["https://dhis2.org/StructureDefinition/MDOrganisationUnitOrganization"]
  },
  "extension" : [{
    "url" : "http://hl7.org/fhir/StructureDefinition/organization-period",
    "valuePeriod" : {
      "start" : "1994-01-01"
    }
  }],
  "identifier" : [{
    "type" : {
      "coding" : [{
        "system" : "http://dhis2.org/identifiertypes",
        "code" : "id"
      }]
    },
    "system" : "http://dhis2.org/identifiertypes#id",
    "value" : "ImspTQPwCqd"
  },
  {
    "type" : {
      "coding" : [{
        "system" : "http://dhis2.org/identifiertypes",
        "code" : "code"
      }]
    },
    "system" : "http://dhis2.org/identifiertypes#code",
    "value" : "OU_525"
  }],
  "name" : "Sierra Leone"
}

```
