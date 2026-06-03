# MDOrganisationUnit Location - DHIS2 Example FHIR Implementation Guide v1.0.0

## Resource Profile: MDOrganisationUnit Location 

 
MDOrganisationUnit Location 

**Usages:**

* Examples for this Profile: [Sierra Leone](Location-MDOrganisationUnitLocation-Sierra-Leone.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-MDOrganisationUnitLocation.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-MDOrganisationUnitLocation.csv), [Excel](../StructureDefinition-MDOrganisationUnitLocation.xlsx), [Schematron](../StructureDefinition-MDOrganisationUnitLocation.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "MDOrganisationUnitLocation",
  "url" : "https://dhis2.org/StructureDefinition/MDOrganisationUnitLocation",
  "version" : "1.0.0",
  "name" : "MDOrganisationUnitLocation",
  "title" : "MDOrganisationUnit Location",
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
  "description" : "MDOrganisationUnit Location",
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
  },
  {
    "identity" : "w5",
    "uri" : "http://hl7.org/fhir/fivews",
    "name" : "FiveWs Pattern Mapping"
  }],
  "kind" : "resource",
  "abstract" : false,
  "type" : "Location",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Location",
  "derivation" : "constraint",
  "differential" : {
    "element" : [{
      "id" : "Location",
      "path" : "Location"
    },
    {
      "id" : "Location.extension",
      "path" : "Location.extension",
      "slicing" : {
        "discriminator" : [{
          "type" : "value",
          "path" : "url"
        }],
        "ordered" : false,
        "rules" : "open"
      },
      "min" : 2
    },
    {
      "id" : "Location.extension:shortName",
      "path" : "Location.extension",
      "sliceName" : "shortName",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Extension",
        "profile" : ["https://dhis2.org/StructureDefinition/ShortName"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "Location.extension:level",
      "path" : "Location.extension",
      "sliceName" : "level",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Extension",
        "profile" : ["https://dhis2.org/StructureDefinition/Level"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "Location.extension:organisationUnitGroup",
      "path" : "Location.extension",
      "sliceName" : "organisationUnitGroup",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "Extension",
        "profile" : ["https://dhis2.org/StructureDefinition/OrganisationUnitGroup"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "Location.extension:attributeValue",
      "path" : "Location.extension",
      "sliceName" : "attributeValue",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "Extension",
        "profile" : ["https://dhis2.org/StructureDefinition/AttributeValue"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "Location.extension:geometry",
      "path" : "Location.extension",
      "sliceName" : "geometry",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Extension",
        "profile" : ["http://hl7.org/fhir/StructureDefinition/location-boundary-geojson"]
      }],
      "mustSupport" : true
    },
    {
      "id" : "Location.identifier",
      "path" : "Location.identifier",
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
      "id" : "Location.identifier:id",
      "path" : "Location.identifier",
      "sliceName" : "id",
      "min" : 1,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Location.identifier:id.type",
      "path" : "Location.identifier.type",
      "min" : 1,
      "patternCodeableConcept" : {
        "coding" : [{
          "system" : "http://dhis2.org/identifiertypes",
          "code" : "id"
        }]
      }
    },
    {
      "id" : "Location.identifier:id.value",
      "path" : "Location.identifier.value",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Location.identifier:code",
      "path" : "Location.identifier",
      "sliceName" : "code",
      "min" : 0,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Location.identifier:code.type",
      "path" : "Location.identifier.type",
      "min" : 1,
      "patternCodeableConcept" : {
        "coding" : [{
          "system" : "http://dhis2.org/identifiertypes",
          "code" : "code"
        }]
      }
    },
    {
      "id" : "Location.identifier:code.value",
      "path" : "Location.identifier.value",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Location.identifier:href",
      "path" : "Location.identifier",
      "sliceName" : "href",
      "min" : 0,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Location.identifier:href.type",
      "path" : "Location.identifier.type",
      "min" : 1,
      "patternCodeableConcept" : {
        "coding" : [{
          "system" : "http://dhis2.org/identifiertypes",
          "code" : "href"
        }]
      }
    },
    {
      "id" : "Location.identifier:href.value",
      "path" : "Location.identifier.value",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Location.name",
      "path" : "Location.name",
      "min" : 1,
      "mustSupport" : true
    },
    {
      "id" : "Location.description",
      "path" : "Location.description",
      "mustSupport" : true
    },
    {
      "id" : "Location.managingOrganization",
      "path" : "Location.managingOrganization",
      "min" : 1,
      "type" : [{
        "code" : "Reference",
        "targetProfile" : ["https://dhis2.org/StructureDefinition/MDOrganisationUnitOrganization"]
      }]
    },
    {
      "id" : "Location.partOf",
      "path" : "Location.partOf",
      "mustSupport" : true
    }]
  }
}

```
