# HIV Initial Case Report - DHIS2 Example FHIR Implementation Guide v1.0.0

## Logical Model: HIV Initial Case Report 

 
Initial case report filled out after enrollment. 

**Usages:**

* Use this Logical Model: [HIV Case Surveillance](StructureDefinition-HIVView.md)

You can also check for [usages in the FHIR IG Statistics](https://packages2.fhir.org/xig/resource/org.hisp.dhis.alldevs.demo|current/StructureDefinition/StructureDefinition-HIVCaseData.json)

### Formal Views of Profile Content

 [Description Differentials, Snapshots, and other representations](http://build.fhir.org/ig/FHIR/ig-guidance/readingIgs.html#structure-definitions). 

 

Other representations of profile: [CSV](../StructureDefinition-HIVCaseData.csv), [Excel](../StructureDefinition-HIVCaseData.xlsx) 



## Resource Content

```json
{
  "resourceType" : "StructureDefinition",
  "id" : "HIVCaseData",
  "url" : "https://dhis2.org/StructureDefinition/HIVCaseData",
  "version" : "1.0.0",
  "name" : "HIVCaseData",
  "title" : "HIV Initial Case Report",
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
  "description" : "Initial case report filled out after enrollment.",
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
  "type" : "https://dhis2.org/StructureDefinition/HIVCaseData",
  "baseDefinition" : "http://hl7.org/fhir/StructureDefinition/Base",
  "derivation" : "specialization",
  "differential" : {
    "element" : [{
      "id" : "HIVCaseData",
      "path" : "HIVCaseData",
      "short" : "HIV Initial Case Report",
      "definition" : "Initial case report filled out after enrollment."
    },
    {
      "id" : "HIVCaseData.initialCaseReportDate",
      "path" : "HIVCaseData.initialCaseReportDate",
      "short" : "Initial Case Report",
      "definition" : "Initial Case Report",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "date"
      }]
    },
    {
      "id" : "HIVCaseData.dateHIVPositiveTest",
      "path" : "HIVCaseData.dateHIVPositiveTest",
      "short" : "Date of documented positive HIV test",
      "definition" : "Date of documented positive HIV test",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "date"
      }]
    },
    {
      "id" : "HIVCaseData.ageWhenDiagnosedWithHiv",
      "path" : "HIVCaseData.ageWhenDiagnosedWithHiv",
      "short" : "Age at diagnosis",
      "definition" : "Age at diagnosis",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "integer"
      }]
    },
    {
      "id" : "HIVCaseData.verticalTransmission",
      "path" : "HIVCaseData.verticalTransmission",
      "short" : "Vertical transmission",
      "definition" : "Vertical transmission",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVCaseData.typeOfTesting",
      "path" : "HIVCaseData.typeOfTesting",
      "short" : "Type of community-level testing",
      "definition" : "Type of community-level testing",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Coding"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "https://dhis2.org/ValueSet/HIVtypeOfTestingVS"
      }
    },
    {
      "id" : "HIVCaseData.facilityLevelTestingEntryPoint",
      "path" : "HIVCaseData.facilityLevelTestingEntryPoint",
      "short" : "Entry point for facility-level testing",
      "definition" : "Entry point for facility-level testing",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "Coding"
      }],
      "binding" : {
        "strength" : "example",
        "valueSet" : "https://dhis2.org/ValueSet/HIVfacilityLevelTestingEntryPointsVS"
      }
    },
    {
      "id" : "HIVCaseData.patientInKeyPopGroup",
      "path" : "HIVCaseData.patientInKeyPopGroup",
      "short" : "Does this person belong to any Key Population groups",
      "definition" : "Does this person belong to any Key Population groups",
      "min" : 1,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVCaseData.keyPopGroupMenWhoHaveSexWithMen",
      "path" : "HIVCaseData.keyPopGroupMenWhoHaveSexWithMen",
      "short" : "Key population - Men who have sex with men",
      "definition" : "Key population - Men who have sex with men",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVCaseData.keyPopGroupInjectionDrugUser",
      "path" : "HIVCaseData.keyPopGroupInjectionDrugUser",
      "short" : "Key population - Injection drug user",
      "definition" : "Key population - Injection drug user",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVCaseData.keyPopGroupPrisoner",
      "path" : "HIVCaseData.keyPopGroupPrisoner",
      "short" : "Key population - Prisoner",
      "definition" : "Key population - Prisoner",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVCaseData.keyPopGroupSexWorker",
      "path" : "HIVCaseData.keyPopGroupSexWorker",
      "short" : "Key population - Sex worker",
      "definition" : "Key population - Sex worker",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    },
    {
      "id" : "HIVCaseData.keyPopGroupTransgender",
      "path" : "HIVCaseData.keyPopGroupTransgender",
      "short" : "Key population - Transgender",
      "definition" : "Key population - Transgender",
      "min" : 0,
      "max" : "1",
      "type" : [{
        "code" : "boolean"
      }]
    }]
  }
}

```
