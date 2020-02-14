This page describes the mapping between the elements in Phenopackets and the resources, profiles and extensions in the Phenopackets on FHIR implementation guide. The mapping was done by looking for the best matching FHIR resources and adding extensions to cover any gaps that were found.

### Building Blocks

| Phenopackets element                                                                             | Comment                                                                                                       |
| ------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------- |
| [Age](https://phenopackets-schema.readthedocs.io/en/latest/age.html)                             | Not needed because FHIR has its own [age](https://www.hl7.org/fhir/datatypes.html#Age) data type.             |
| [AgeRange](https://phenopackets-schema.readthedocs.io/en/latest/age.html#agerange)               | Not needed because FHIR has its own [range](https://www.hl7.org/fhir/datatypes.html#Range) data type.         |
| [Biosample](https://phenopackets-schema.readthedocs.io/en/latest/biosample.html)                 | Corresponds to the [Biosample](StructureDefinition-Biosample.html) profile.               |
| [Disease](https://phenopackets-schema.readthedocs.io/en/latest/disease.html)                     | Corresponds to the [Disease](StructureDefinition-Disease.html) profile.                                       |
| [Evidence](https://phenopackets-schema.readthedocs.io/en/latest/evidence.html)                   | Corresponds to the [Evidence](StructureDefinition-Evidence.html) extension.                                   |
| [ExternalReference](https://phenopackets-schema.readthedocs.io/en/latest/externalreference.html) | Corresponds to the [External Reference](StructureDefinition-ExternalReference.html) extension.               |
| [Gene](https://phenopackets-schema.readthedocs.io/en/latest/gene.html)                           | Corresponds to [ObsRegionStudied](http://build.fhir.org/ig/HL7/genomics-reporting/region-studied.html) in the [FHIR Genomics Reporting Implementation Guide](http://build.fhir.org/ig/HL7/genomics-reporting/index.html). |
| [HtsFile](https://phenopackets-schema.readthedocs.io/en/latest/file.html)                        | Corresponds to the [Hts File](StructureDefinition-HtsFile.html) profile.                                      |
| [Individual](https://phenopackets-schema.readthedocs.io/en/latest/individual.html)               | Corresponds to the [Individual](StructureDefinition-Individual.html) profile.                                 |
| [Karyotypic sex](https://phenopackets-schema.readthedocs.io/en/latest/karyotypicsex.html)        | Corresponds to the [individual karyotypic sex](StructureDefinition-KaryotypicSex.html) extension. |
| [Metadata](https://phenopackets-schema.readthedocs.io/en/latest/metadata.html)                   | Not needed because FHIR already has its own metadata infrastructure.                                          |
| [OntologyClass](https://phenopackets-schema.readthedocs.io/en/latest/ontologyclass.html)         | Not needed because FHIR already has comprehensive support for terminologies.                                  |
| [Pedigree](https://phenopackets-schema.readthedocs.io/en/latest/pedigree.html)                   | Corresponds to the [Pedigree Node](StructureDefinition-PedigreeNode.html) profile.                            |
| [PhenotypicFeature](https://phenopackets-schema.readthedocs.io/en/latest/phenotype.html)         | Corresponds to the [Phenotypic Feature](StructureDefinition-PhenotypicFeature.html) profile.                  |
| [Procedure](https://phenopackets-schema.readthedocs.io/en/latest/procedure.html)                 | Corresponds to [Specimen.collection](https://www.hl7.org/fhir/specimen-definitions.html#Specimen.collection). |
| [Resource](https://phenopackets-schema.readthedocs.io/en/latest/resource.html)                   | Not needed because FHIR already has comprehensive support for terminologies.                                  |
| [Sex](https://phenopackets-schema.readthedocs.io/en/latest/sex.html)                             | Not needed because FHIR already has the _gender_ attribute in the Patient resource.                           |
| [Variant](https://phenopackets-schema.readthedocs.io/en/latest/variant.html)                     | Corresponds to [Variant](http://build.fhir.org/ig/HL7/genomics-reporting/variant.html) in the [FHIR Genomics Reporting Implementation Guide](http://build.fhir.org/ig/HL7/genomics-reporting/index.html). |

### Top-level Elements

| Phenopackets element                                                                       | Comment                                                                               |
| ------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------- |
| [Phenopacket](https://phenopackets-schema.readthedocs.io/en/latest/phenopacket.html)       | Corresponds to the [Phenopackets](StructureDefinition-Phenopacket.html) profile.      |
| [Family](https://phenopackets-schema.readthedocs.io/en/latest/family.html)                 | Corresponds to the [Family](StructureDefinition-Family.html) profile.                 |
| [Cohort](https://phenopackets-schema.readthedocs.io/en/latest/cohort.html)                 | Corresponds to the [Cohort](StructureDefinition-Cohort.html) profile.                 |
| [Interpretation](https://phenopackets-schema.readthedocs.io/en/latest/interpretation.html) | Corresponds to the [Interpretation](StructureDefinition-Interpretation.html) profile. |
