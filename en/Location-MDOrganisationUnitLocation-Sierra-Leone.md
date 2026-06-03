# MDOrganisationUnitLocation-Sierra-Leone - DHIS2 Example FHIR Implementation Guide v1.0.0

## Example Location: MDOrganisationUnitLocation-Sierra-Leone

Profile: [MDOrganisationUnit Location](StructureDefinition-MDOrganisationUnitLocation.md)

**ShortName**: Sierra Leone

**MDOrganisationUnit Hiearchy Level**: 1

**identifier**: id/ImspTQPwCqd, code/OU_525

**name**: Sierra Leone

**managingOrganization**: `MDOrganisationUnitOrganization/ImspTQPwCqd`



## Resource Content

```json
{
  "resourceType" : "Location",
  "id" : "MDOrganisationUnitLocation-Sierra-Leone",
  "meta" : {
    "profile" : ["https://dhis2.org/StructureDefinition/MDOrganisationUnitLocation"]
  },
  "extension" : [{
    "url" : "https://dhis2.org/StructureDefinition/ShortName",
    "valueString" : "Sierra Leone"
  },
  {
    "url" : "https://dhis2.org/StructureDefinition/Level",
    "valueInteger" : 1
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
  "name" : "Sierra Leone",
  "managingOrganization" : {
    "reference" : "MDOrganisationUnitOrganization/ImspTQPwCqd"
  }
}

```
