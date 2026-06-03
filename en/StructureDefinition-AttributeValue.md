# MDAttributeValue - DHIS2 Example FHIR Implementation Guide v1.0.0

## Extension: MDAttributeValue 

MDAttributeValue Extension

**Context of Use**

**Usage info**

**Usages:**

* Use this Extension: [MDOrganisationUnit Location](StructureDefinition-MDOrganisationUnitLocation.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-AttributeValue.json)

### Formal Views of Extension Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-AttributeValue.csv), [Excel](../StructureDefinition-AttributeValue.xlsx), [Schematron](../StructureDefinition-AttributeValue.sch) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "AttributeValue",
  "url" : "https://dhis2.org/StructureDefinition/AttributeValue",
  "version" : "1.0.0",
  "name" : "AttributeValue",
  "title" : "MDAttributeValue",
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
  "description" : "MDAttributeValue Extension",
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
      "short" : "MDAttributeValue",
      "definition" : "MDAttributeValue Extension"
    },
    {
      "id" : "Extension.extension",
      "path" : "Extension.extension",
      "min" : 2
    },
    {
      "id" : "Extension.extension:attribute",
      "path" : "Extension.extension",
      "sliceName" : "attribute",
      "short" : "MDAttribute UID",
      "min" : 1,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Extension.extension:attribute.extension",
      "path" : "Extension.extension.extension",
      "max" : "0"
    },
    {
      "id" : "Extension.extension:attribute.url",
      "path" : "Extension.extension.url",
      "fixedUri" : "attribute"
    },
    {
      "id" : "Extension.extension:attribute.value[x]",
      "path" : "Extension.extension.value[x]",
      "type" : [{
        "code" : "Coding"
      }]
    },
    {
      "id" : "Extension.extension:value",
      "path" : "Extension.extension",
      "sliceName" : "value",
      "short" : "MDAttribute Value",
      "min" : 1,
      "max" : "1",
      "mustSupport" : true
    },
    {
      "id" : "Extension.extension:value.extension",
      "path" : "Extension.extension.extension",
      "max" : "0"
    },
    {
      "id" : "Extension.extension:value.url",
      "path" : "Extension.extension.url",
      "fixedUri" : "value"
    },
    {
      "id" : "Extension.extension:value.value[x]",
      "path" : "Extension.extension.value[x]",
      "type" : [{
        "code" : "string"
      }]
    },
    {
      "id" : "Extension.url",
      "path" : "Extension.url",
      "fixedUri" : "https://dhis2.org/StructureDefinition/AttributeValue"
    },
    {
      "id" : "Extension.value[x]",
      "path" : "Extension.value[x]",
      "max" : "0"
    }]
  }
}

```
