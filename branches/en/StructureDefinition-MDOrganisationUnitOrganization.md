# MDOrganisationUnit Organization - DHIS2 Example FHIR Implementation Guide v1.0.0

## Resource Profile: MDOrganisationUnit Organization 

 
MDOrganisationUnit Organization 

**Usages:**

* Refer to this Profile: [MDOrganisationUnit Location](StructureDefinition-MDOrganisationUnitLocation.md)
* Examples for this Profile: [Sierra Leone](Organization-MDOrganisationUnitOrganization-Sierra-Leone.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-MDOrganisationUnitOrganization.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-MDOrganisationUnitOrganization.csv), [Excel](../StructureDefinition-MDOrganisationUnitOrganization.xlsx), [Schematron](../StructureDefinition-MDOrganisationUnitOrganization.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "MDOrganisationUnitOrganization",
  "url" : "https://dhis2.org/StructureDefinition/MDOrganisationUnitOrganization",
  "version" : "1.0.0",
  "name" : "MDOrganisationUnitOrganization",
  "title" : "MDOrganisationUnit Organization",
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
  "description" : "MDOrganisationUnit Organization",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "mapping" : [{
    "identity" : "v2",
    "uri" : "http://hl7.org/v2",
    "name" : "HL7 v2 Mapping"
  },
  {
    "identity" : "rim",
    "uri" : "http://hl7.org/v3",
    "name" : "RIM Mapping"
  },
  {
    "identity" : "servd",
    "uri" : "http://www.omg.org/spec/ServD/1.0/",
    "name" : "ServD"
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Organization",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Organization",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Organization",
      "path" : "Organization"
    },
    {
      "id" : "Organization.extension",
      "path" : "Organization.extension",
      "slicing" : {
        "discriminator" : [{
          "type" : "value",
          "path" : "url"
        }],
        "ordered" : false,
        "rules" : "open"
      },
      "min" : 1
    },
    {
      "id" : "Organization.extension:openingDate",
      "path" : "Organization.extension",
      "sliceName" : "openingDate",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Extension",
        "profile" : ["http://hl7.org/fhir/StructureDefinition/organization-period"]
      }]
    },
    {
      "id" : "Organization.extension:openingDate.value[x].start",
      "path" : "Organization.extension.value[x].start",
      "min" : 1
    },
    {
      "id" : "Organization.extension:openingDate.value[x].end",
      "path" : "Organization.extension.value[x].end",
      "max" : "0"
    },
    {
      "id" : "Organization.identifier",
      "path" : "Organization.identifier",
      "slicing" : {
        "discriminator" : [{
          "type" : "pattern",
          "path" : "type"
        }],
        "description" : "DHIS2 Unique Identifier",
        "ordered" : false,
        "rules" : "open"
      },
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Organization.identifier:id",
      "path" : "Organization.identifier",
      "sliceName" : "id",
      "min" : 1,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Organization.identifier:id.type",
      "path" : "Organization.identifier.type",
      "min" : 1,
      "patternCodeableConcept" : {
        "coding" : [{
          "system" : "http://dhis2.org/identifiertypes",
          "code" : "id"
        }]
      }
    },
    {
      "id" : "Organization.identifier:id.value",
      "path" : "Organization.identifier.value",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Organization.identifier:code",
      "path" : "Organization.identifier",
      "sliceName" : "code",
      "min" : 0,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Organization.identifier:code.type",
      "path" : "Organization.identifier.type",
      "min" : 1,
      "patternCodeableConcept" : {
        "coding" : [{
          "system" : "http://dhis2.org/identifiertypes",
          "code" : "code"
        }]
      }
    },
    {
      "id" : "Organization.identifier:code.value",
      "path" : "Organization.identifier.value",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Organization.identifier:href",
      "path" : "Organization.identifier",
      "sliceName" : "href",
      "min" : 0,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Organization.identifier:href.type",
      "path" : "Organization.identifier.type",
      "min" : 1,
      "patternCodeableConcept" : {
        "coding" : [{
          "system" : "http://dhis2.org/identifiertypes",
          "code" : "href"
        }]
      }
    },
    {
      "id" : "Organization.identifier:href.value",
      "path" : "Organization.identifier.value",
      "min" : 1,
      "mustSupport" : true
    }]
  }
}

```
