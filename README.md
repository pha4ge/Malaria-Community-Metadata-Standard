# Malaria Community Metadata Standard (MCMS)– Collection template and associated materials for malaria metadata

Publication(s) DOI. [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)



## Malaria contextual data specification overview

Public health genomics contextual data for malaria integrates epidemiological, clinical, geographic, laboratory, and sequencing metadata. This contextual data enables interpretation of genomic surveillance outputs, informs malaria control and elimination strategies, reveals parasite population dynamics, resistance emergence, and transmission patterns, and facilitates scientific understanding of malaria disease. Standardized contextual data supports data integration, reuse, and public health decision‑making across surveillance systems.

The malaria contextual data specification addresses gaps in existing general (MIxS) and pathogen‑specific standards by capturing malaria‑specific complexities – vector ecology, transmission dynamics, and health system factors in endemic settings. Supporting materials include harmonized collection templates for human clinical/One Health and mosquito vector samples, controlled vocabularies, reference guides, and mapping to existing standards. All resources are openly available and detailed below.

## Content description

### Malaria contextual data specification package

Spreadsheet-based (.xlsx) [human clinical/One Health collection template](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MalariaCommunityMetadataStandard_human_samples_v2_0_0.xlsx);
Spreadsheet-based (.xlsx) [mosquito vector collection template](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MalariaCommunityMetadataStandard_mosquito_samples_v2_0_0.xlsx).

Core components (Spreadsheet tabs):
1. **Data collection template:**

A structured sheet for entering full metadata sets, featuring "required" fields (yellow), "strongly recommended" fields (purple) and "optional" fields (white).

2. **User reference guide:**

Detailed instructions, field definitions, population tips, and real-world examples to streamline template completion.

3. **Controlled vocabulary lists**

Malaria experts-approved; ontology-linked term lists for dropdown selection, promoting consistent data entry.

#### [Machine-Readable JSON Template](https://github.com/pha4ge/malaria-data-spec-json)

An automated JSON version of the MCMS template, optimized for programmatic use. “Required” fields are enforced as mandatory, while “strongly recommended” and “optional” fields remain non-mandatory (with minor adjustments due to JSON constraints).

### Standard operating procedure (SOP)

Step-by-step guidelines for template use, term selection, sample description formatting, and key considerations for ethics, practicality, and data privacy. The SOP is available at [Malaria contextual metadata SOP](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MCMS_contextual_data_SOP.md).

### Supporting materials

[**MCMS to PHA4GE SARS-CoV-2 contextual data specification field mappings:**](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MCMS_v2_0_0_human_Mapping_to_PHA4GE_to_INSDC.xlsx)

Aligns MCMSs fields with the SARS-CoV-2 metadata for genomic surveillance.

[**MCMS to MPOX metadata specification field mappings:**](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MCMS_v2_0_0_human_Mapping_to_PHA4GE_to_INSDC.xlsx)

Aligns MCMSs fields with the MPOX metadata for genomic surveillance.

[**MCMS to Repository field mappings:**](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MCMS_v2_0_0_human_Mapping_to_PHA4GE_to_INSDC.xlsx)

Crosswalks MCMS fields to submission forms for ENA and NCBI, facilitating data export and transformation.

## JSON Specification Generation

Machine-readable [JSON schemas](https://github.com/pha4ge/malaria-data-spec-json) for MCMS are generated automatically from CSV versions of the templates, using the `malaria_table_json.py` script in the [MCMS JSON repository](https://github.com/pha4ge/malaria-data-spec-json). There is one schema for each template:

| Template | CSV | JSON schema |
|:--|:--|:--|
| [Human clinical/One Health](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MalariaCommunityMetadataStandard_human_samples_v2_0_0.xlsx) | [CSV](https://github.com/pha4ge/malaria-data-spec-json/blob/main/MalariaCommunityMetadataStandard_human_samples_v2_0_0_with_required_optional.csv) | [PHA4GE_Malaria_Contextual_Data_Schema_Human.json](https://github.com/pha4ge/malaria-data-spec-json/blob/main/PHA4GE_Malaria_Contextual_Data_Schema_Human.json) |
| [Mosquito vector](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MalariaCommunityMetadataStandard_mosquito_samples_v2_0_0.xlsx) | [CSV](https://github.com/pha4ge/malaria-data-spec-json/blob/main/MalariaCommunityMetadataStandard_mosquito_samples_v2_0_0_with_required_optional.csv) | [PHA4GE_Malaria_Contextual_Data_Schema_Mosquito.json](https://github.com/pha4ge/malaria-data-spec-json/blob/main/PHA4GE_Malaria_Contextual_Data_Schema_Mosquito.json) |

### Generating the schemas

1. **Export the CSV.** Save the **Field Reference Guide** sheet of the template as a CSV with the columns in Table 1. Keep one row per field and remove the section-header rows. Set the `Required/Optional` column from the colour of the field name: yellow is "Required", purple is "Recommended" and white is "Optional".
2. **Run the tool.** It requires Python 3.7 or later:

```bash
git clone https://github.com/pha4ge/malaria-data-spec-json.git
cd malaria-data-spec-json

python malaria_table_json.py MalariaCommunityMetadataStandard_human_samples_v2_0_0_with_required_optional.csv \
  -o PHA4GE_Malaria_Contextual_Data_Schema_Human.json

python malaria_table_json.py MalariaCommunityMetadataStandard_mosquito_samples_v2_0_0_with_required_optional.csv \
  -o PHA4GE_Malaria_Contextual_Data_Schema_Mosquito.json
```

3. **Check the output.** The tool prints the number of properties and required fields. For MCMS v2.0.0 this should be 229 properties (13 required) for the human schema and 250 properties (12 required) for the mosquito schema.

When a template is updated, regenerate both the CSV and the schema, and commit them to the [MCMS JSON repository](https://github.com/pha4ge/malaria-data-spec-json).

**Table 1** MCMS field specification (CSV columns)

| Column | Description |
|:--|:--|
| Field | Field name, as used for the column headers in the MCMS template. |
| Required/Optional | Requirement level according to the MCMS specification. Limited to the values "Optional", "Recommended" and "Required". |
| Ontology ID | Ontology term identifier associated with the field. |
| Type of Variable(s) | Expected value type, e.g. "Alphanumeric", "Numeric", "Free text", "Structured format" or "Permitted value(s)". Fields that accept more than one pick-list value are marked "multiselect". |
| Definition | Short description of the expected field value. |
| Guidance | Detailed guidance for accurately completing the field. |
| Example(s) | Example of a valid field value. |

In the generated schema, each field name becomes a snake_case property key. "Numeric" fields become numbers, "multiselect" fields become lists of values, date fields use the ISO 8601 date format (YYYY-MM-DD), and all other fields are text. Only "Required" fields are enforced. See the [MCMS JSON repository README](https://github.com/pha4ge/malaria-data-spec-json#readme) for full details.

## Contacts

For support, reach out to`help@pha4ge.org` or the repository's issue tracker.

## Acknowledgement

Abhinav Sharma, Alan Christoffels, Andrew Balmer, Arsene Bokulu, Bacha Mekonen, Bernard Aniakwo Logonia, Bernardete Rafael, Betselot Z Ayano, Charmaine Matimba, Christoph Cyranski, David Oladejo, Dilyet Girmay, Dominique Anderson, Tafese Beyene Tufa, Eddie Tshikala Lulamba, Emilyn Costa Conceicao, Emma Griffiths, Francis Farai Chikuse, Francis Mubigalo, Hannah Faber, Hannah Jauncey, Jaishree Raman, Jennie Lee, John Magudha, Katairo Thomas, Kedir Abdella Abdulsemed, Latifah Mukanga, Lauren Fromont, Mehul Dhorda, Michele A Miller, Michelle Parker, Nalia Ismael, Nawaal Weitz, Nicholas Hathaway, Nina White, Palesa Makoti, Paulo Arnaldo, Prince Asare, Rekha Sathyan, Richard Pearson, Sarah Cooke, Selam Yirga, Stanford Kwenda, Stefanie Hatchell, Susan Alicia Fisher, Tahita Marc Christian, Victoire Nsabatien, Vito Baraka, on behalf of the Public Health Alliance for Genomic Epidemiology (PHA4GE) consortium and GenEpi Network/Data Standards & Data Integration working group.

## Citation


## License

[MIT License](LISENCE.md)
