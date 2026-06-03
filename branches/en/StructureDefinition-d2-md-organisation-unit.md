# DHIS2 Metadata: OrganisationUnit - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: DHIS2 Metadata: OrganisationUnit 

 
DHIS2 Metadata: OrganisationUnit 

**Usages:**

* This Logical Model is not used by any profiles in this Specification

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-d2-md-organisation-unit.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-d2-md-organisation-unit.csv), [Excel](../StructureDefinition-d2-md-organisation-unit.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "d2-md-organisation-unit",
  "url" : "https://dhis2.org/StructureDefinition/d2-md-organisation-unit",
  "version" : "1.0.0",
  "name" : "MDOrganisationUnit",
  "title" : "DHIS2 Metadata: OrganisationUnit",
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
  "description" : "DHIS2 Metadata: OrganisationUnit",
  "jurisdiction" : [{
    "coding" : [{
      "system" : "http://unstats.un.org/unsd/methods/m49/m49.htm",
      "code" : "001",
      "display" : "World"
    }]
  }],
  "fhirVersion" : "4.0.1",
  "kind" : "logical",
  "abstract" : false,
  "type" : "https://dhis2.org/StructureDefinition/d2-md-organisation-unit",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "d2-md-organisation-unit",
      "path" : "d2-md-organisation-unit",
      "short" : "DHIS2 Metadata: OrganisationUnit",
      "definition" : "DHIS2 Metadata: OrganisationUnit"
    },
    {
      "id" : "d2-md-organisation-unit.id",
      "path" : "d2-md-organisation-unit.id",
      "short" : "Unique UID for organisation unit",
      "definition" : "Unique UID for organisation unit",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.code",
      "path" : "d2-md-organisation-unit.code",
      "short" : "Unique CODE for organisation unit",
      "definition" : "Unique CODE for organisation unit",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.href",
      "path" : "d2-md-organisation-unit.href",
      "short" : "Unique URL where the organisation unit is available from",
      "definition" : "Unique URL where the organisation unit is available from",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.level",
      "path" : "d2-md-organisation-unit.level",
      "short" : "Level in hiearchy of organisation units",
      "definition" : "Level in hiearchy of organisation units",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "integer"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.parent",
      "path" : "d2-md-organisation-unit.parent",
      "short" : "Parent of organisation unit",
      "definition" : "Parent of organisation unit",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.leaf",
      "path" : "d2-md-organisation-unit.leaf",
      "short" : "Is this is a leaf node in the organisation unit tree",
      "definition" : "Is this is a leaf node in the organisation unit tree",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.name",
      "path" : "d2-md-organisation-unit.name",
      "short" : "Name of organisation",
      "definition" : "Name of organisation",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.shortName",
      "path" : "d2-md-organisation-unit.shortName",
      "short" : "Short name of organisation unit",
      "definition" : "Short name of organisation unit",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.description",
      "path" : "d2-md-organisation-unit.description",
      "short" : "Description of organisation unit",
      "definition" : "Description of organisation unit",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.openingDate",
      "path" : "d2-md-organisation-unit.openingDate",
      "short" : "Date this organisation unit was opened",
      "definition" : "Date this organisation unit was opened",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "date"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.geometry",
      "path" : "d2-md-organisation-unit.geometry",
      "short" : "GeoJson geometry of organisation unit",
      "definition" : "GeoJson geometry of organisation unit",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.organisationUnitGroups",
      "path" : "d2-md-organisation-unit.organisationUnitGroups",
      "short" : "organisation unit groups that contains this organisation unit",
      "definition" : "organisation unit groups that contains this organisation unit",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.dataSets",
      "path" : "d2-md-organisation-unit.dataSets",
      "short" : "data sets associated with this organisation unit",
      "definition" : "data sets associated with this organisation unit",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.programs",
      "path" : "d2-md-organisation-unit.programs",
      "short" : "programs associated with this organisation unit",
      "definition" : "programs associated with this organisation unit",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "Identifier"
      }]
    },
    {
      "id" : "d2-md-organisation-unit.attributeValues",
      "path" : "d2-md-organisation-unit.attributeValues",
      "short" : "additional attributes that are in this organisation unit",
      "definition" : "additional attributes that are in this organisation unit",
      "min" : 0,
      "max" : "*",
      "type" : [{
        "code" : "https://dhis2.org/StructureDefinition/d2-md-attribute-value"
      }]
    }]
  }
}

```
