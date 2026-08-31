**Malaria Community Standard – Collection template and associated materials for malaria metadata**

Publication(s) DOI(s).

**Malaria contextual data specification overview**

Public health genomics contextual data for malaria integrates epidemiological, clinical, geographic, laboratory, and sequencing metadata. This contextual data enables interpretation of genomic surveillance outputs, informs malaria control and elimination strategies, reveals parasite population dynamics, resistance emergence, and transmission patterns, and facilitates scientific understanding of malaria disease. Standardized contextual data supports data integration, reuse, and public health decision‑making across surveillance systems.

The malaria contextual data specification addresses gaps in existing general (MIxS) and pathogen‑specific standards by capturing malaria‑specific complexities – vector ecology, transmission dynamics, and health system factors in endemic settings. Supporting materials include harmonized collection templates for human clinical/One Health and mosquito vector samples, controlled vocabularies, reference guides, and mapping to existing standards. All resources are openly available and detailed below.

**Content description**

**Malaria contextual data specification package**

Spreadsheet-based (.xlsx) human clinical/One Health collection template (link)

Spreadsheet-based (.xlsx) mosquito vector collection template (link)

Core components (Spreadsheet tabs):

1. **Data collection template**: A structured sheet for entering full metadata sets, featuring "required" fields (yellow), "strongly recommended" fields (purple) and "optional" fields (white).
2. **User reference guide:** Detailed instructions, field definitions, population tips, and real-world examples to streamline template completion.
3. **Controlled vocabulary lists:** Malaria experts/PHA4GE-approved; ontology-linked term lists for dropdown selection, promoting consistent data entry.

**Machine-Readable JSON Template (link)**

An automated JSON version of the MCS template, optimized for programmatic use. "Required" fields are enforced as mandatory, while "strongly recommended" and "optional" fields remain non-mandatory (with minor adjustments due to JSON constraints).

**Standard operating procedure (SOP)**

Step-by-step guidelines for template use, term selection, sample description formatting, and key considerations for ethics, practicality, and data privacy. **Available at…** (link).

**Supporting materials**

- **MCS to PHA4GE SARS-CoV-2 contextual data specification field mappings (link):** Aligns MCSs fields with the SARS-CoV-2 metadata for genomic surveillance.
- **MCS to MPOX metadata specification field mappings (link):** Aligns MCSs fields with the MPOX metadata for genomic surveillance.
- **MCS to Repository field mappings (link):** Crosswalks MCS fields to submission forms for ENA and NCBI, facilitating data export and transformation.

**JSON Specification Generation**

The JSON schema (link) is generated automatically from a csv template (link) via scripts in MCS JSON repository (link).

**Table 1 MCS field specification**

| **Column**        | **Description**                                                                   |
| ----------------- | --------------------------------------------------------------------------------- |
| Interface Label   | Header names in the MCS template.                                                 |
| ---               | ---                                                                               |
| Required/Optional | Classification as "Required," "Recommended," or "Optional" per MCS standards.     |
| ---               | ---                                                                               |
| Definition        | Concise explanation of the field's purpose.                                       |
| ---               | ---                                                                               |
| Ontology          | Associated ontology identifier.                                                   |
| ---               | ---                                                                               |
| Value Type        | Permitted formats: (e.g., "String," "Date," "Integer_or_Range," "BioProject_ID"). |
| ---               | ---                                                                               |
| Example           | Sample valid entry.                                                               |
| ---               | ---                                                                               |
| Guidance          | In-depth notes for accurate completion.                                           |
| ---               | ---                                                                               |

**Acknowledgment**

Abhinav Sharma, Alan Christoffels, Andrew Balmer, Arsene Bokulu, Bacha Mekonen, Bernard Aniakwo Logonia, Bernardete Rafael, Betselot Z Ayano, Charmaine Matimba, Christoph Cyranski, David Oladejo, Dilyet Girmay, Dominique Anderson, Tafese Beyene Tufa, Eddie Tshikala Lulamba, Emilyn Costa Conceicao, Emma Griffiths, Francis Farai Chikuse, Francis Mubigalo, Hannah Faber, Hannah Jauncey, Jaishree Raman, Jennie Lee, John Magudha, Katairo Thomas, Kedir Abdella Abdulsemed, Latifah Mukanga, Lauren Fromont, Mehul Dhorda, Michele A Miller, Michelle Parker, Nalia Ismael, Nawaal Weitz, Nicholas Hathaway, Nina White, Palesa Makoti, Paulo Arnaldo, Prince Asare, Rekha Sathyan, Richard Pearson, Sarah Cooke, Selam Yirga, Stanford Kwenda, Stefanie Hatchell, Susan Alicia Fisher, Tahita Marc Christian, Victoire Nsabatien, Vito Baraka, on behalf of the Public Health Alliance for Genomic Epidemiology (PHA4GE) consortium and GenEpi Network/Data Standards & Data Integration working group.

**Contacts**

For support, reach out to [elulamba@pha4ge.org](mailto:elulamba@pha4ge.org) or the repository's issue tracker.

**Citation**

Tshikala Eddie Lulamba, Dominique Anderson, Francis Mubigalo, Bacha Mekonen, Susan Alicia Fisher, Nalia Ismael, Stanford Kwenda, Vito Baraka, Francis Farai Chikuse, Jaishree Raman, Mehul Dhorda, Nicholas Hathaway, Emma Griffiths, Nina White, Hannah Jauncey, Bernardete Rafael, Jennie Lee, David Oladejo, Andrew Balmer, Paulo Arnaldo, Sarah Cooke, Richard Pearson, Stephanie Van Wyk, Thomas Katairo, Alan Christoffels (DOI)

**License**

[MIT License.]([url](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/main/LICENSE))
