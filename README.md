**Readme**

**Malaria-Community-Metadata-Standard**

**Overview**

Malaria remains a major cause of morbidity and mortality globally, with the highest burden borne by countries in sub-Saharan Africa. Malaria epidemiology is increasingly influenced by the emergence and spread of antimalarial drug resistance in *Plasmodium falciparum* and insecticide resistance in *Anopheles* vectors, threatening recent gains in control. Genomic surveillance has therefore become central to monitoring parasite population structure, detecting resistance-associated mutations and haplotypes, and informing evidence-based control and elimination strategies. Advances in whole-genome sequencing (WGS) and other high-throughput genomic technologies have transformed our ability to investigate transmission dynamics and track the geographic spread of resistance. However, the full value of malaria genomic data can only be realized when it is accompanied by high-quality, harmonized, and context-aware metadata.

This repository contains the **Malaria Community Metadata Standard**, a structured and interoperable framework designed to support malaria genomic surveillance and epidemiology. The standard aims to enable consistent data capture, improve interoperability across studies and platforms, and facilitate meaningful comparison, integration, and reuse of malaria genomic datasets across endemic settings.

**Background**

**Malaria**

Malaria is a life-threatening parasitic disease caused by protozoa of the genus *Plasmodium* and transmitted to humans through the bites of infected female *Anopheles* mosquitoes. Five *Plasmodium* species infect humans, with *P. falciparum* and *P. vivax* responsible for the greatest global burden. *Plasmodium* *falciparum* accounts for most severe disease and mortality, particularly in sub-Saharan Africa, while *P. vivax* predominates in many regions outside Africa. Clinical presentations range from uncomplicated febrile illness to severe complications such as profound anaemia, respiratory distress, cerebral malaria, and multiorgan failure. Young children, pregnant women, travellers, and immunocompromised individuals remain at highest risk. Despite significant progress in control efforts, malaria continues to cause hundreds of millions of cases and over half a million deaths annually, with the overwhelming majority occurring in the African Region.

Malaria epidemiology is increasingly shaped by heterogeneous transmission dynamics and by the emergence and spread of antimalarial drug resistance in *P. falciparum* and insecticide resistance in *Anopheles* vectors, threatening recent gains in control. Genomic epidemiology has therefore become a critical tool to:

* Characterize parasite population structure and genetic diversity
* Detect and monitor resistance-associated mutations and haplotypes
* Track transmission patterns and cross-border spread
* Inform targeted control and elimination strategies.

Large volumes of *Plasmodium* genomic data are now available through global repositories and surveillance networks. However, robust metadata describing the hosts, epidemiological context, geographic and temporal factors, sample characteristics, and laboratory and analytical processes and results are essential to interpret genomic findings accurately and to place them within meaningful public health and transmission contexts. Without standardized and harmonized contextual data, malaria genomic datasets remain difficult to integrate, compare, and reuse across studies, regions, and surveillance systems.

**Metadata Standards in Genomic Epidemiology**

Metadata standards define a common structure, vocabulary, and set of expectations for describing data. In genomic epidemiology, standardized metadata:

* Improves data quality and completeness
* Enables interoperability across databases, tools, and studies
* Facilitates data sharing and reuse in line with FAIR principles (Findable, Accessible, Interoperable, Reusable)
* Supports reproducibility and transparent interpretation of results

Without standardized metadata, genomic datasets are difficult to integrate, compare, or interpret beyond their original study context. Developing a domain-specific metadata standard for malaria ensures that critical clinical and epidemiological variables are captured in a consistent and meaningful way.

**Scope**

This metadata standard is intended to support malaria genomic surveillance and epidemiological studies by defining a harmonized set of metadata elements covering infecting Plasmodium species; diverse sample and host types; associated clinical, epidemiological, and laboratory data; tiled amplicon, targeted (e.g., bait-capture), and shotgun metagenomic sequencing approaches; and genotyping information. The standard is designed for use in research, public health surveillance, and data-sharing initiatives.

This standard:

* Focuses on metadata accompanying pathogen genomic data related to malaria
* Is applicable across diverse geographic, laboratory, and healthcare settings
* Supports retrospective and prospective genomic studies

This standard is **not** intended to:

* Replace clinical diagnostic criteria or treatment guidelines
* Serve as a comprehensive electronic health record schema
* Function as a regulatory or clinical decision-support tool

**Purpose of This Repository**

This repository serves as the authoritative home for the Malaria Community Metadata Standard and its supporting materials. It is intended for use by researchers, clinicians, public health professionals, and data stewards working in genomic epidemiology and malaria health.

Specifically, this repository aims to:

* Provide a clear and well-documented metadata specification for malaria genomic surveillance and epidemiological studies
* Support consistent implementation of the standard across projects and institutions
* Enable testing, validation, and iterative improvement of the standard
* Promote transparency and community engagement in standard development.

**Repository Contents**

This repository includes the following components:

* **Metadata Dictionaries** The core definition of the malaria metadata standard, including fields, descriptions, data types, and controlled vocabularies where applicable.
* **Metadata Template** Metadata template in Excel format to support implementation and adoption by users.
* **Documentation** Supporting documentation explaining design decisions, scope, assumptions, and intended use cases.
* **Versioning and Change History** Records of updates, revisions, and known issues to support traceability and long-term maintenance.

**Intended Audience**

This repository is intended for:

* Genomic epidemiology researchers studying malaria
* Clinical and public health teams generating or using pathogen genomic data
* Bioinformaticians and data managers implementing metadata standards
* Standards developers and stakeholders interested in malaria health data harmonization

**Contributing and Feedback**

Contributions, feedback, and issue reports are welcome. Community input is essential to ensure the metadata standard remains relevant, practical, and scientifically robust. Please see the contribution guidelines for details on how to get involved.

**Citation**

If you use, adapt, or reference this metadata standard in your work, please credit:

**Public Health Alliance for Genomic Epidemiology (PHA4GE)**

A formal citation and citation file (CITATION.cff) may be added in future releases.

**License**

License information is provided in this repository.
