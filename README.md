# Malaria Community Standard – Collection template and associated materials for malaria metadata

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)



## PHA4GE overview

The Public Health Alliance for Genomic Epidemiology ([PHA4GE](https://pha4ge.org)) is a global coalition that is actively working to establish consensus standards, document and share best practices, improve the availability of critical bioinformatic tools and resources, and advocate for greater openness, interoperability, accessibility and reproducibility in public health microbial bioinformatics.

In the face of the current SARS-CoV-2 pandemic, [PHA4GE](https://pha4ge.org) has identified a clear and present need for a fit-for-purpose, open source SARS-CoV-2 contextual data standard. As such, we have developed a SARS-CoV-2 contextual data specification based on harmonizable, publicly available, community standards.

## Malaria contextual data specification overview
Public health genomics contextual data for malaria integrates epidemiological, clinical, geographic, laboratory, and sequencing metadata. This contextual data enables interpretation of genomic surveillance outputs, informs malaria control and elimination strategies, reveals parasite population dynamics, resistance emergence, and transmission patterns, and facilitates scientific understanding of malaria disease. Standardized contextual data supports data integration, reuse, and public health decision‑making across surveillance systems.

The malaria contextual data specification addresses gaps in existing general (MIxS) and pathogen‑specific standards by capturing malaria‑specific complexities – vector ecology, transmission dynamics, and health system factors in endemic settings. Supporting materials include harmonized collection templates for human clinical/One Health and mosquito vector samples, controlled vocabularies, reference guides, and mapping to existing standards. All resources are openly available and detailed below.

## Content description

### Malaria contextual data specification package

#### [Spreadsheet-based (.xlsx) human clinical/One Health collection template](MalariaCommunityStandard_human_v2_0_0.xlsx)

#### [Spreadsheet-based (.xlsx) mosquito vector collection template](MalariaCommunityStandard_mosquito_v2_0_0.xlsx)

It contains the following items (tabs in the spreadsheet):

1. **Data collection template:**

A structured sheet for entering full metadata sets, featuring "required" fields (yellow), "strongly recommended" fields (purple) and "optional" fields (white).

2. **User reference guide:**

Detailed instructions, field definitions, population tips, and real-world examples to streamline template completion.

3. **Controlled vocabulary lists**

Malaria experts/PHA4GE-approved; ontology-linked term lists for dropdown selection, promoting consistent data entry.

#### [Machine-Readable JSON Template](https://github.com/pha4ge/malaria-data-spec-json)

An automated JSON version of the MCS template, optimized for programmatic use. *Required* fields are enforced as mandatory, while *strongly recommended* and *optional* fields remain non-mandatory (with minor adjustments due to JSON constraints).

### Standard operating procedure (SOP)

Step-by-step guidelines for template use, term selection, sample description formatting, and key considerations for ethics, practicality, and data privacy. The SOP is available at [Malaria contextual metadata SOP](MCS_contextual_data_SOP.md).

### Supporting materials

[**MCS to PHA4GE SARS-CoV-2 contextual data specification field mappings:**](#)

Aligns MCSs fields with the SARS-CoV-2 metadata for genomic surveillance.

[**MCS to MPOX metadata specification field mappings:**](#)

Aligns MCSs fields with the MPOX metadata for genomic surveillance.

[**MCS to Repository field mappings:**](#)

Crosswalks MCS fields to submission forms for ENA and NCBI, facilitating data export and transformation.

## JSON Specification Generation

The [JSON schema](#) is generated automatically from a [csv template](#) via scripts in [MCS JSON repository](https://github.com/pha4ge/malaria-data-spec-json).


**Table 1** MCS field specification

| Column | Description |
|:-:|:-:|
| Interface Label | Column headers in the MCS template. |
| Required/Optional | Type of requirement according to the MCS specification. Limited to the values "Optional", "Recommended", and "Required". |
| Definition | Short description of the expected interface label value. |
| Ontology | Ontology ID associated with the interface label. |
| Value Type | Expected interface label value type. Permitted values include "String", "Date", "Integer_or_Range", and "BioProject_ID". |
| Example | Example of a valid interface label value. |
| Guidance | Detailed guidance for accurately completing the expected interface label value. |                                  |

## Contacts

For support, reach out to`elulamba@pha4ge.org` or the repository's issue tracker..

## Acknowledgement

Abhinav Sharma, Alan Christoffels, Andrew Balmer, Arsene Bokulu, Bacha Mekonen, Bernard Aniakwo Logonia, Bernardete Rafael, Betselot Z Ayano, Charmaine Matimba, Christoph Cyranski, David Oladejo, Dilyet Girmay, Dominique Anderson, Tafese Beyene Tufa, Eddie Tshikala Lulamba, Emilyn Costa Conceicao, Emma Griffiths, Francis Farai Chikuse, Francis Mubigalo, Hannah Faber, Hannah Jauncey, Jaishree Raman, Jennie Lee, John Magudha, Katairo Thomas, Kedir Abdella Abdulsemed, Latifah Mukanga, Lauren Fromont, Mehul Dhorda, Michele A Miller, Michelle Parker, Nalia Ismael, Nawaal Weitz, Nicholas Hathaway, Nina White, Palesa Makoti, Paulo Arnaldo, Prince Asare, Rekha Sathyan, Richard Pearson, Sarah Cooke, Selam Yirga, Stanford Kwenda, Stefanie Hatchell, Susan Alicia Fisher, Tahita Marc Christian, Victoire Nsabatien, Vito Baraka, on behalf of the Public Health Alliance for Genomic Epidemiology (PHA4GE) consortium and GenEpi Network/Data Standards & Data Integration working group.

## Citation
Tshikala Eddie Lulamba, Dominique Anderson, Francis Mubigalo, Bacha Mekonen, Susan Alicia Fisher, Nalia Ismael, Stanford Kwenda, Vito Baraka, Francis Farai Chikuse, Jaishree Raman, Mehul Dhorda, Nicholas Hathaway, Emma Griffiths, Nina White, Hannah Jauncey, Bernardete Rafael, Jennie Lee, David Oladejo, Andrew Balmer, Paulo Arnaldo, Sarah Cooke, Richard Pearson, Stephanie Van Wyk, Thomas Katairo, Alan Christoffels (DOI)

## License

[MIT License](LISENCE.md)
