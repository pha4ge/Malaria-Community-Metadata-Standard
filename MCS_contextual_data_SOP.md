# Malaria contextual metadata SOP

**Tshikala Eddie Lulamba¹, Susan Alicia Fernol**  
¹ University of the Western Cape, South African National Bioinformatics Institute

## Disclaimer

Please note that this protocol is public domain, which supersedes the CC-BY license default used by protocols.io.

## Abstract

The systematic curation of contextual information is essential for malaria genomic surveillance, public health investigations, and responsible data stewardship. It helps preserve the long-term value, interoperability, and reusability of genomic and epidemiological datasets.

This protocol presents guidance for organizing malaria-related information using the Malaria Community Standard contextual data collection template, with the aim of improving consistency and harmonization across laboratories, surveillance initiatives, datasets, and information systems.

The template comprises a data-entry collection template, a field reference guide containing definitions, guidance and examples, and a sheet of controlled vocabularies that support the use of consistent terminology.

The protocol also outlines procedures for completing and validating the template and highlights some ethical, privacy, governance, and operational issues that should be considered with the appropriate data steward before data sharing takes place. Supporting appendices provide examples and recommendations for describing types of malaria samples, and identify additional standardized terms when necessary.

> **Note:** Before distributing any information recorded in the template, data providers should consult relevant jurisdictional and organizational data-sharing requirements.

A PDF version of this SOP is available here: [Link to the PDF version](https://github.com/pha4ge/Malaria-Community-Metadata-Standard/blob/v0.1/MCS_contextual_data_SOP_pdf_v1.pdf#:~:text=MCS_contextual_data_SOP.md-,MCS_contextual_data_SOP_pdf_v1,-.pdf)

For more information and/or assistance, contact [elulamba@pha4ge.org](mailto:elulamba@pha4ge.org).

---

## I. Purpose

To structure malaria contextual data across *Plasmodium* and *Anopheles* species in line with global pathogen metadata frameworks, including PHA4GE pathogen standards, to enable harmonization and interoperability across datasets, countries, and systems.

a. Data providers will curate malaria contextual data in accordance with the procedures described below.

b. Data providers will complete the harmonized metadata template with information from their datasets using applicable picklists and prescribed instructions.

c. Data providers may share harmonized malaria metadata in accordance with applicable national legislation, jurisdictional requirements, and organizational data governance and access policies, including tiered or restricted sharing where applicable.

---

## II. Scope

This SOP applies to the standardization, collection, validation, and management of contextual data associated with malaria genomic datasets for *Plasmodium* and *Anopheles* species.

### Intended users

- Researchers and research institutions.
- Public health laboratories and surveillance programs.
- Data curators and data managers.
- Malaria data-sharing organizations.

### Out of scope

- Software and/or database implementation.
- Bioinformatics pipelines or genomic data analysis workflows.
- Detailed legal, ethical, or regulatory frameworks (compliance required).
- Non-*Plasmodium* pathogens.

---

## III. Data

The types of information that can be captured in the template include:

1. Identifiers and repository accession numbers;
2. Sample collection and processing;
3. Strain and isolate information;
4. Environmental measurements and conditions;
5. Host information;
6. Second-host information;
7. Host vaccination information;
8. Host exposure information;
9. Host reinfection information;
10. Sequencing information;
11. Bioinformatics and QC metrics;
12. Taxonomic identification and variant calling information;
13. Marker genotype information; and
14. Contributor acknowledgements.

---

## IV. Populating and curating the template

### 1. Download the template

Download the Malaria Metadata Collection Template (Excel and JSON) and the Reference Guide from the project GitHub repository:

[Link to GitHub repository for template](#)

### 2. Pre-curation review

Before populating data:

- Review your dataset.
- Review the fields and expected values in the collection template.
- Review the Reference Guide for field definitions and guidance.

### 3. Confirm mappings with your data steward or supervisor

- Map each local dataset field to the corresponding standardized metadata fields in the template.
- Agree on the level of detail (granularity) appropriate for public versus restricted sharing, following institutional policies and applicable data-governance frameworks.

> **Note:** Maintain two versions where required: a detailed version for internal use and a generalized version for public release. Prioritise inclusion of maximum allowable detail while respecting privacy, ethics, and regulatory constraints.

### 4. Populate the template

Enter dataset information into the template following these priorities:

- **Mandatory fields** (colour-coded yellow) should be completed first.
- **Recommended fields** (colour-coded purple) should be completed where data are available and permitted.
- **Optional fields** (colour-coded white) may be completed where relevant and permitted.

#### Guidelines

- Use provided controlled vocabularies and picklists whenever available.
- Adhere to prescribed formats, e.g., date formats, address formats, and geographic naming conventions.
- Ensure consistency and accuracy across all entries.
- Store data securely in accordance with institutional data-protection procedures.

> **Note — Missing or restricted data:** If a field is not applicable or data cannot be shared, use standardized null values to indicate the reason, e.g., `"not collected"`, `"not applicable"`, or `"restricted"`.

### Required fields

| Subsection | Required Fields |
|---|---|
| Sample Collection and Processing |  |
| Host Information | Host (scientific name)<br>Host disease |
| Bioinformatics and QC Metrics | Consensus sequence software name<br>Consensus sequence software version |

### 5. Reference and validation

- Use the Reference Guide for complete field guidance.
- Use Appendix A for ethics and privacy considerations.
- Use Appendix B for sample matrices.
- Use Appendix C for ontology searching.
- For missing standardized terms in a picklist, use Appendix C to source terms from ontology lookup services.

### 6. Submission (Optional)

Submit sequences and accompanying metadata to relevant public or consortia repositories as permitted:

- **AGARI** — *Plasmodium* species tracking.
- **INSDC repositories** — sequence archiving and public access.

---

## V. Appendix A: Ethical, practical, and privacy considerations

Effective and equitable malaria responses depend on timely and sustained international collaboration and data sharing. The Malaria Community Standard supports consistent collection, integration, and sharing of high-quality data across diverse surveillance settings and research purposes.

Many metadata elements in this standard are essential for public health use but may raise ethical, practical, or privacy concerns that should be addressed before data are shared. Users of this specification should comply with applicable data-governance frameworks and local laws, as requirements vary by jurisdiction (e.g., GDPR in Europe, POPIA in South Africa) and by data type (clinical versus vector samples).

Consult data stewards, privacy officers, and institutional policies, and refer to the Reference Guide for field-level guidance.

> **Note:** This guidance draws on the PHA4GE pathogen contextual data specification and is not intended to cover all possible scenarios or use cases. Users, in consultation with data providers and data stewards, are responsible for determining how best to implement this specification in their own contexts. Where the collected information is intended for research, additional administrative and ethical requirements, such as review by a Research Ethics Board (REB) or equivalent ethics committee, will typically apply.

### Identifiers and repository accession numbers

Sharing *Plasmodium* genomic sequences, including raw reads, assemblies and consensus genomes, together with contextual data in public repositories, facilitates the monitoring of malaria transmission dynamics, phylogeographic analyses, surveillance of resistance-associated molecular markers, and studies of vector competence.

Laboratories worldwide submit malaria data to public repositories, including INSDC partner databases (ENA, NCBI, and DDBJ), as well as MalariaGEN, PlasmoDB and AGARI, while capturing minimal contextual data to support interoperability.

Upon submission to a public repository, accession numbers are assigned as unique identifiers for tracking, retrieval, and version control. Depending on what is shared and how it is shared, INSDC partner repositories may assign different accession numbers.

Assemblies and consensus sequences may be submitted to GenBank or equivalent databases, raw sequence data to the Sequence Read Archive (SRA), and contextual data as BioSample records. Information may also be organized within BioProjects, including higher-level Umbrella BioProjects (see Reference Guide for further information). All applicable accession numbers should be recorded.

Data generated by or submitted to MalariaGEN, PlasmoDB, and AGARI may also be submitted to INSDC partner databases. AGARI may additionally assign accession numbers to BioProjects, BioSamples, and raw, assembled (processed), and/or consensus sequences.

Malaria sample workflows often involve multiple agencies, from field collection to laboratory processing, sequencing, and public health application. Comprehensive records should therefore be maintained for all identifiers associated with samples, specimens, sequencing libraries, hosts, and sequence data (raw, processed, or consensus), where applicable and permitted.

Tracking these identifiers supports traceability, chain-of-custody, reproducibility, and follow-up. Although the metadata standard includes fields for commonly used identifiers, these fields may not capture every identifier required for specific workflows. Users should record all relevant identifiers, even where additional fields must be added, and should maintain internal consistency across datasets and submissions.

Some identifiers may be sensitive or classified as public health identifiable information (PHII), particularly in low-prevalence settings. Prior to sharing, the appropriate authority should be consulted to determine whether specific identifiers may be released publicly.

Where identifiers are sensitive, de-identified identifiers should be used for sharing and the mapping keys stored separately with restricted access, or the null value `"restricted"` should be applied for sensitive fields, as specified in the Reference Guide.

### Geographical information

Geographical metadata, including country, subnational administrative divisions, and precise coordinates, is essential for mapping *Plasmodium* transmission across multiple spatial scales.

For human clinical samples, detailed geographic information may constitute PHII, particularly in low-prevalence or elimination settings, and may therefore require abstraction before public release.

Where permitted, geographic fields in the metadata template, including subnational administrative levels, sample collection location, host residence location, and likely location of exposure, should be completed. Additional fields may be incorporated, where necessary, to capture relevant geographic information in accordance with the metadata standard.

Each geographic field should be assigned to the appropriate context.

**Sample collection location** refers to the place where the specimen was obtained and may include country, subnational administrative divisions, and precise coordinates, where permissible. These may include:

- `geo_loc_name (country)`
- `first-order_administrative_division`
- `second-order_administrative_division`
- `third-order_administrative_division`
- `fourth-order_administrative_division`
- `geo_loc_latitude`
- `geo_loc_longitude`
- `altitude`
- `depth`

**Host residence location** refers to the location where the host resides and may be recorded as:

- `host_residence_geo_loc_name (country)`

**Location of exposure** refers to the location where infection was most likely acquired and may be recorded using:

- `location_of_exposure_geo_loc_name (country)`
- `destination_of_most_recent_travel (country)`
- `destination_of_most_recent_travel (state/province/territory)`
- `destination_of_most_recent_travel (city)`
- `travel_history`

Curators should ensure that each field is used in relation to the sample, the host residence, or the likely exposure location, as applicable.

Prior to sharing geographic data, particularly in public repositories, users should confirm the permitted level of detail with data stewards or relevant authorities.

Geographic granularity should be reduced where necessary, for example by reporting country or first-order administrative division rather than exact coordinates.

Where latitude and longitude are shared, they should correspond to the actual sampling location, where allowed. Proxy locations, such as city centres, institutional addresses, or other substituted points, must not be used, as they may misrepresent the data and lead to incorrect interpretation.

Fields related to host residence location and location of exposure may be particularly sensitive in malaria-endemic settings and may increase the risk of re-identification, especially in small communities, low-prevalence areas, or vulnerable populations.

At the same time, these data are important for distinguishing imported from local transmission, identifying spatial disparities, and supporting analyses of multi-species malaria dynamics.

Users should also consider the broader ethical implications of geographic metadata, including the potential for stigmatization of communities, reinforcement of inequities in data generation and use, and limitation of equitable access to the benefits of data use.

Particular care is required when working with underserved or marginalized populations, Indigenous communities, and settings with limited healthcare infrastructure.

Prior to submission to a public repository such as ENA or NCBI, users should confirm compliance with applicable privacy and governance requirements. For sensitive geographic fields, the null value `"restricted"` should be used in accordance with the Reference Guide, balancing surveillance needs with privacy protection.

### Date information

Temporal metadata, including `sample_collection_date`, `sequencing_date`, and `symptom_onset_date`, are important for malaria surveillance and research.

Such data support analyses of transmission dynamics, seasonality, outbreak detection, and the evaluation of intervention strategies across all *Plasmodium* species.

Dates may be considered sensitive or may constitute PHII, particularly when combined with detailed geographic information, associated with small populations or low case counts, or linked to other identifiable metadata.

Before sharing temporal data, users should assess the risk of re-identification and confirm the permissible level of detail with data stewards or relevant authorities.

Accurate temporal information, particularly the sample collection date, is highly valuable for downstream analyses; however, where exact dates are considered sensitive, they may be generalized to the month or year, or offset ("jittered") by a small number of days for de-identification purposes.

Any such modifications should be applied only to the shared dataset and not to the original records. Original dates must be retained securely for traceability and internal use.

Temporal logic should be verified to ensure consistency, for example, that collection precedes receipt and sequencing.

In some instances, specific date fields, such as `sample_collection_date`, may not be available to the data submitter, may require additional permissions to access, or may be difficult to obtain because of operational or logistical constraints.

In such cases, `sample_received_date` may be used as a proxy, provided that its use is clearly documented.

### Purpose of sampling / Purpose of sequencing

Sampling strategies can influence malaria datasets and may introduce bias.

A sample may be collected for one purpose and later selected for another, e.g., collected for diagnostic testing and subsequently sequenced for surveillance, research, or outbreak investigation.

Information on why samples were collected and why they were selected for sequencing, including whether selection was random or targeted, supports interpretation of the data and downstream epidemiological analyses.

Standardized terms should be used where available in the `purpose_of_sampling` field, such as:

- Diagnostic testing
- Research
- Surveillance

Standardized terms should also be used in the `purpose_of_sequencing` field, such as:

- Routine surveillance
- Variant or marker monitoring
- Cluster or outbreak investigation
- Baseline surveillance

Additional context may be recorded in:

- `purpose_of_sampling_details`
- `purpose_of_sequencing_details`

The Reference Guide should be consulted for suggested wording and examples relevant to common malaria surveillance and research activities.

### Host information

Beyond basic species identification (*Homo sapiens*), human host metadata associated with malaria samples should generally be treated as PHII and handled with appropriate safeguards before public release.

Such information is usually collected at the point of care or specimen collection and is typically retained by the institution responsible for the original sample. Access may require specific authorization and may be constrained by operational factors such as workload, system access, or manual curation requirements.

Common host variables in malaria surveillance include age and sex, which support epidemiological analysis and linkage between laboratory and field data.

Although these variables may not be directly identifying on their own, they may become identifiable when combined with other contextual information such as geographic location or collection date.

To reduce re-identification risk, age may be reported in predefined ranges (bins), such as:

- 0–9 years
- 10–19 years
- 20–29 years
- 30–39 years
- 40–49 years
- 50–59 years
- 60–69 years
- 70–79 years
- 80–89 years
- 90–99 years
- 100+ years

Clinical host metadata may include symptomatic or asymptomatic infection status, disease severity, treatment status, and outcome, where available and permitted.

These data may be recorded using structured fields, such as:

- `host_health_state`
- `host_health_state_details`

Detailed individual-level information, including symptoms, comorbidities, risk factors, and complications, should be generalized or aggregated where sharing is permitted.

### Host exposure information

Exposure information is important for understanding malaria transmission patterns and informing public health action.

In malaria, exposure is usually linked to the bite of an infected *Anopheles* mosquito, environmental conditions that support vector presence, and human movement between endemic and non-endemic areas.

Relevant information may include:

- Likely location of exposure.
- Travel history.
- Ecological setting, e.g., rural versus urban.
- Occupational or behavioural factors, such as outdoor nighttime activities, that may increase risk.

This information is often highly sensitive because it may reveal travel patterns, specific communities, workplaces, or other locations, and may increase the risk of re-identification when combined with dates or geographic metadata.

Despite these sensitivities, exposure information is valuable for distinguishing local from imported malaria cases, identifying transmission hotspots and high-risk environments, and supporting targeted vector control and intervention strategies.

Users should confirm the permissible level of detail with data stewards or relevant authorities and use aggregated or generalized descriptions where appropriate.

### Methods information

Methodological metadata, including sampling design, laboratory protocols, bioinformatics workflows, and quality control metrics, provides essential context for interpreting *Plasmodium* genomic data, assessing bias, and supporting reproducible malaria analyses.

Comprehensive and well-structured methodological information should be recorded to support:

- Correct biological and epidemiological interpretation.
- Reproducibility.
- Quality assurance and control.
- Long-term data reuse.

Methodological information should be recorded in a structured and standardized format wherever possible.

Relevant methods should be documented at the time of data generation and analysis rather than retrospectively.

Where protocols are extensive, they may be summarized within metadata fields and supplemented with references to external documents or publications.

Wherever feasible and permitted, methodological details should be recorded using standardized fields and controlled vocabularies, including software names, versions, and parameter settings to support reproducibility, and stored in a centralized and accessible location alongside the metadata.

### Null values

Standardized null value reporting is important for maintaining data quality, transparency, and interoperability.

When a value cannot be provided for a required or expected metadata field, controlled vocabulary terms should be used to indicate why the data are absent.

The International Nucleotide Sequence Database Collaboration (INSDC) set of standardized null value terms should be used to distinguish among the main reasons a value may be unavailable:

| Null value | Meaning |
|---|---|
| `Not Applicable` | The field does not apply to the sample. |
| `Missing` | The value is expected but is not currently available. |
| `Not Collected` | The data were not collected. |
| `Not Provided` | The data exist but are not shared. |
| `Restricted Access` | The data are sensitive and cannot be shared publicly. |

Users should provide as much metadata as possible wherever feasible and permitted, and null values should be used only when necessary.

Blank fields should be avoided.

The selected null value should reflect the most specific applicable reason for the missing data, and null values should be applied consistently across the dataset.

---

## VI. Appendix B: Describing your sample

The context in which a sample was collected, including why, how, when, and where it was obtained, directly affects the interpretation of *Plasmodium* genomic data.

Temporal and geographic information supports transmission analysis, while provenance records help establish the chain-of-custody.

Sampling differences, such as passive clinic-based case detection versus reactive detection, variation in parasitemia across specimen types, and laboratory passage, should be documented to support accurate cluster interpretation and mutation validation.

Sampling context and methods influence:

- Parasite density and detectability.
- Sequencing success and data quality.
- Detection of mixed infections.
- Interpretation of transmission patterns.

Where possible, users should record relevant metadata using standardized fields, including purpose of sampling, specimen processing methods, laboratory host or culture system, and passage information.

Passage information should indicate:

- Whether parasites were cultured or passaged before sequencing.
- The number of passages.
- The method used.

Malaria samples may originate from a range of sources, including human clinical samples, One Health samples, and mosquito samples.

To support consistent description, standardized fields may include:

- Anatomical material.
- Anatomical part.
- Body product.
- Environmental material.
- Related sample descriptors.

Users should complete only those fields that apply to the sample type and should provide the most detailed level of information permitted by applicable data-sharing policies.

### Example: Human capillary whole blood sample

| Host (scientific name) | Host (common name) | Host disease | Anatomical material | Anatomical part | Collection device |
|---|---|---|---|---|---|
| *Homo sapiens* | Human | Malaria | Whole blood | Capillary blood | Filter paper |

### Example: Human venous whole blood sample

| Host (scientific name) | Host (common name) | Host disease | Anatomical material | Anatomical part | Collection device |
|---|---|---|---|---|---|
| *Homo sapiens* | Human | Malaria | Whole blood | Venous blood | Vacutainer with K2EDTA |

### Example: Human brain tissue collected post-mortem

| Host (scientific name) | Host (common name) | Host disease | Host health outcome | Anatomical material | Collection device |
|---|---|---|---|---|---|
| *Homo sapiens* | Human | Cerebral malaria | Deceased | Brain tissue | Vial |

### Example: Animal feces

| Host (scientific name) | Host (common name) | Host disease | Anatomical product | Collection device |
|---|---|---|---|---|
| *Macaca fascicularis* | Long-tailed macaque | Malaria | Feces | Filter paper |

### Example: Adult mosquito sample

| Host (scientific name) | Host (common name) | Second host health state | Anatomical part | Collection device |
|---|---|---|---|---|
| *Anopheles gambiae* | Anopheles mosquito | Healthy, Sporozoite-positive, Parous | Adult, mosquito, whole organism | Centers for Disease Control and Prevention light trap |

### Example: Mosquito tissue sample

| Host (scientific name) | Host (common name) | Second host health state | Anatomical material | Collection device |
|---|---|---|---|---|
| *Anopheles gambiae* | Anopheles mosquito | Healthy, Sporozoite-positive, Parous | Embryonic tissue | Egg paper, oviposition paper, fine mesh sieve |

### Example: Stagnant water for vector surveillance

| Breeding habitat | Environmental material |
|---|---|
| Stagnant canal | Stagnant water |

---

## VII. Appendix C: How to find standardized terms

Standardized vocabularies are essential for ensuring consistency, interoperability, and comparability of malaria metadata across datasets and studies.

Where possible, users should select terms from the standardised picklists provided in the Metadata Collection Template. These picklists may be updated over time to reflect user feedback and evolving standards.

If a required term is not available in the provided picklists, users should identify an appropriate standardized term from a recognized ontology.

1. Access the [EBI Ontology Lookup Service (OLS)](https://www.ebi.ac.uk/ols) and navigate to the ontology resources listed in the SOP Reference Guide, such as EnvO and IDOMAL.
2. Enter the term of interest into the search bar. The closest matching standardized terms will be displayed.
3. Review the results and select the term that most closely matches the intended meaning. Copy the selected term into the relevant field in the metadata template.
4. If no suitable term is identified, search for synonyms or related terms, broaden the search using the general ontology lookup interface, or consult alternative relevant ontologies where appropriate.

### Example workflow

**Term:** `insecticide-treated net`  
**Field:** `infectious_disease_control_strategy`

1. Navigate to the relevant ontology page in the EBI Ontology Lookup Service, for example [IDOMAL](https://www.ebi.ac.uk/ols4/ontologies/idomal).
2. Search for `"insecticide-treated net"` and select the standardized term that best matches the intended meaning, for example `insecticide-treated net (IDOMAL:0000259)`.
3. Open the **Term Reference Guide** sheet in the template.
4. Copy the exact ontology term into the appropriate field in the metadata template.
5. Insert the term alphabetically into the relevant controlled vocabulary list, for example in the `infectious_disease_control_strategy` column.
6. Return to the main data-entry sheet and update data validation to reflect the revised picklist.
7. Save the template and document the update for transparency and reproducibility.

Additionally:

- Record any additions to the picklist for transparency and reproducibility.
- Where applicable, notify collaborators or data managers of the update.

### Key ontologies for malaria metadata

| Ontology | Application |
|---|---|
| **IDOMAL** | Health, malaria-specific concepts, and control interventions |
| **EnvO** | Environmental and vector collection sites |
| **NCBITaxon** | Vector taxonomy |
| **UBERON** | Anatomical parts, e.g., midgut and salivary glands |
| **MIxS extensions** | Sequencing and QC metrics |
| **SNOMED** | Clinical terms |

**Figure 1.** Example of using the EBI Ontology Lookup Service to identify standardized terms, showing the list of suggested matches returned from a search query.

For more information and/or assistance, contact [elulamba@pha4ge.org](mailto:elulamba@pha4ge.org).

---

## Revision History

| Version | Date | Writer | Description of change |
|---|---|---|---|
| 0.0 | August 31, 2026 | Tshikala Eddie Lulamba, Susan Alicia Fernol | Created protocol |
|  |  |  |  |
