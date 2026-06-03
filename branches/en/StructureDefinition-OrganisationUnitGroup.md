# MDOrganisationUnitGroup Identifier - DHIS2 Example FHIR Implementation Guide v1.0.0

## Extension: MDOrganisationUnitGroup Identifier 

MDOrganisationUnitGroup Identifier Extension

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [MDOrganisationUnit Location](StructureDefinition-MDOrganisationUnitLocation.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-OrganisationUnitGroup.json)

### Formal Views of Extension Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-OrganisationUnitGroup.csv), [Excel](../StructureDefinition-OrganisationUnitGroup.xlsx), [Schematron](../StructureDefinition-OrganisationUnitGroup.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "OrganisationUnitGroup",
  "url" : "https://dhis2.org/StructureDefinition/OrganisationUnitGroup",
  "version" : "1.0.0",
  "name" : "OrganisationUnitGroup",
  "title" : "MDOrganisationUnitGroup Identifier",
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
  "description" : "MDOrganisationUnitGroup Identifier Extension",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  }],
  "kind" : "complex-type",
  "abstract" : false,
  "context" : [{
    "type" : "element",
    "expression" : "Element"
  }],
  "type" : "Extension",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Extension",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Extension",
      "path" : "Extension",
      "short" : "MDOrganisationUnitGroup Identifier",
      "definition" : "MDOrganisationUnitGroup Identifier Extension"
    },
    {
      "id" : "Extension.extension",
      "path" : "Extension.extension",
      "max" : "0"
    },
    {
      "id" : "Extension.url",
      "path" : "Extension.url",
      "fixedUri" : "https://dhis2.org/StructureDefinition/OrganisationUnitGroup"
    },
    {
      "id" : "Extension.value[x]",
      "path" : "Extension.value[x]",
      "type" : [{
        "code" : "Identifier"
      }]
    }]
  }
}

```
