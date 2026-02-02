*(To be filled in and uploaded as deliverable in the Portal Grant Management System, at the due date foreseen in the system (and regularly updated).*

*(The template is recommended but not mandatory. If you do not use it, please make however sure that you comply with the research data management requirements under Article 17 of the Grant Agreement.)*

| PROJECT |  |
| :---- | :---- |
| **Project number:** | 01186579  |
| **Project acronym:** | EUCENTRAL |
| **Project name:** | Modelling Center for Quantum Technologies |

| DATA MANAGEMENT PLAN |  |
| :---- | :---- |
| **Date**: | 02.02.2026 |
| **Version:** | 2.0 |

## Glossary of Terms

1. **TR:** The Trusted Repository. In this case the Zenodo repository.

2. **CR:** The Code Repository. In this case, Github.

3. **LR:** The Local Repository. In this case, the locally hosted server at CFT PAN.

4. **DMP:** This Data Management Plan.

5. **GA:** The Grant Agreement.

## 1. Data Summary

**Q. Will you re-use any existing data and what will you re-use it for? State the reasons if re-use of any existing data has been considered but discarded.** 

No existing data will be reused.

**Q. What types and formats of data will the project generate or re-use?**

The project will generate representations of a quantum mechanical wave-functions and associated supplemantary data such as quantum observables.
All data must be stored either in human readable plaintext file formats (such as `.txt`, `.json`) or one of the following allowed binary formats:

- [HDF5](https://github.com/HDFGroup/hdf5) (`.h5`, `.hdf5`)
- [Warsaw Data Format](https://gitlab.fizyka.pw.edu.pl/wtools/wslda/-/wikis/W-data%20format) (`.wdat`)

In the event that one of the above two binary formats is unsuitable, an alternative *open-source* format may be used provided adequate justification is provided to the Data Steward. In this case, the data must be accompanied by details (included version, required packages) of a language environment that can load such a format. 

Figures generated from the data will be exported as both a printable image format (.png) and a scalable vector graphics format (.pdf). 

**Q. What is the purpose of the data generation or re-use and its relation to the objectives of the project?**

The data is as result of numerical simulations of quantum mechanical systems. The purpose of the data is to provide insights into the quantum many-body problem. Such insights can then be used to a) inform experiment and b) advance theoretical understanding. Specifically, data will be used in the publication of peer-reviewed research articles. 

**Q. What is the expected size of the data that you intend to generate or re-use?**

Across the 5 year project, the total size of the data generated is expected to be no more than 10TiB.

**Q. What is the origin/provenance of the data, either generated or re-used?**

All data is generated as both input and output of numerical simulations.

**Q. To whom might your data be useful ('data utility'), outside your project?**

The data will be useful to researchers who wish to perform further analysis on the outputs of the data, and for peers to review and verify the results of published numerical work.

## 2. FAIR data

### 2.1 Making data findable, including provisions for metadata

**Q. Will data be identified by a persistent identifier?**

Data will be assigned a DOI by the TR. Standalone software will not be assigned a DOI by default as the CR does not assign DOI. Instead, the CR repository name forms the unique identifier for codebases stored at the CR. This allows the code to be published in journals, where a DOI may be assigned upon publication.

**Q. Will rich metadata be provided to allow discovery? What metadata will be created? What disciplinary or general standards will be followed? In case metadata standards do not exist in your discipline, please outline what type of metadata will be created and how.**

Metadata will adhere to the Dublin Core (DCMT) standard. 

**Q. Will search keywords be provided in the metadata to optimize the possibility for discovery and then potential re-use?**

Keywords will be used when required by publications associated with the data. When required by publication, there will be a one-to-one correspondence between the data keywords and the publication keywords.

**Q. Will metadata be offered in such a way that it can be harvested and indexed?** 

All metadata is exported via the OAI-PMH protocol (Open Archives Initiative Protocol for Metadata Harvesting) and can be harvested in accordance with TR policy.

### 2.2 Making data accessible

> Repository:

**Q. Will the data be deposited in a trusted repository?**

Data will be stored in the TR. The TR is hosted and managed by CERN, which has extensive experience in operating large-scale data repositories. The CERN project is funded for the next 20 years, and the TR will be maintained for as long as the project remains funded.

Code will be stored publicly in the CR. The CR is the most widely used repository for code storage and version control and is already routinely used by many researchers.  

**Q. Have you explored appropriate arrangements with the identified repository where your data will be deposited?** 

Not applicable as the TR and the CR are free to use by the public.

**Q. Does the repository ensure that the data is assigned an identifier? Will the repository resolve the identifier to a digital object?** 

The TR assigns a DOI to each set of data, which will be used as the identifier. Furthermore, the TR allows versioning of data. 

> Data:

**Q. Will all data be made openly available? If certain datasets cannot be shared (or need to be shared under restricted access conditions), explain why, clearly separating legal and contractual reasons from intentional restrictions. Note that in multi-beneficiary projects it is also possible for specific beneficiaries to keep their data closed if opening their data goes against their legitimate interests or other constraints as per the Grant Agreement.**

All data used in publication will be made openly available. 

**Q. If an embargo is applied to give time to publish or seek protection of the intellectual property (e.g. patents), specify why and how long this will apply, bearing in mind that research data should be made available as soon as possible.**

Not applicable.

**Q. Will the data be accessible through a free and standardized access protocol?**

According to TR policy, “access to metadata and data files is provided over standard protocols such as HTTP and OAI-PMH”.

**Q. If there are restrictions on use, how will access be provided to the data, both during and after the end of the project?**

There are no restrictions on the use of the data.

**Q. How will the identity of the person accessing the data be ascertained?**

Not applicable.

**Q. Is there a need for a data access committee (e.g. to evaluate/approve access requests to personal/sensitive data)?**

As data is not sensitive or personal, all requests will be granted by the Data Steward automatically.

> Metadata:

**Q. Will metadata be made openly available and licenced under a public domain dedication CC0, as per the Grant Agreement? If not, please clarify why. Will metadata contain information to enable the user to access the data?** 

Yes data will be licensed under CC0 as per both the GA and the TR policy and is openly available.

**Q. How long will the data remain available and findable? Will metadata be guaranteed to remain available after data is no longer available?**

Data and accompanying metadata will be made available for as long as it can be hosted at the TR. Data will also be hosted at CFT PAN offline at the LR for the duration of the project plus an additional 5 years at a minimum. At the end of period, an assessment of the current data storage capabilities by the Data Steward will take place to evaluate for how long the data can be stored going forward. Metadata will be stored seperately at the LR and will remain for as long as reasonably possible, potentially beyond the duration of the associated data, such that data in the TR can be referenced by the LR.

**Q. Will documentation or reference about any software be needed to access or read the data be included? Will it be possible to include the relevant software (e.g. in open source code)?**

All data will be fully reproducible via scripts included in the repository, with an accompanying README file on how to do so. Any code required by the data developed as part of the Project is hosted at an accompanying open-source code base repository at the CR.

### 2.3 Making data interoperable

**Q. What data and metadata vocabularies, standards, formats or methodologies will you follow to make your data interoperable to allow data exchange and re-use within and across disciplines? Will you follow community-endorsed interoperability best practices? Which ones?** 

Data will be stored as human readable plaintext or as [HDF5](https://github.com/HDFGroup/hdf5) (`.h5`, `.hdf5`). HDF5 is standard data storage format for heterogeneous data readable by a wide variety of different software and programming languages. Alternatively, data can be used stored using the open source and documented. [Warsaw Data Format](https://gitlab.fizyka.pw.edu.pl/wtools/wslda/-/wikis/W-data%20format) (`.wdat`) as this is a commonly used format at IF PAN. Metadata will adhere to Dublin Core standard. 

**Q. In case it is unavoidable that you use uncommon or generate project specific ontologies or vocabularies, will you provide mappings to more commonly used ontologies? Will you openly publish the generated ontologies or vocabularies to allow reusing, refining or extending them?**

All mappings will be published and included in the data repository. 

**Q. Will your data include qualified references[^1] to other data (e.g. other data from your project, or datasets from previous research)?**

Qualified references will be used where appropriate including references to any known work published using the data, and any further data derived from the data. These references can be included in the TR.

### 2.4 Increase data re-use

**Q. How will you provide documentation needed to validate data analysis and facilitate data re-use (e.g. readme files with information on methodology, codebooks, data cleaning, analyses, variable definitions, units of measurement, etc.)?**

All data used in publication must be reproducible as a requirement for publication. Data reproducibility is ensured by:

1. Any physical variables appearing in data and data-generating code must be accompanied with physical units as a code comment (if unitful). All non-derivative (input) variables must be accompanied by a code comment explaining their function. 

2. A source code (non-binary) script(s) must be included in the data repository that can reproduce the data. 

3. Any binary files produced and required to produce the data must be accompanied with the source code and details on how the binary can be generated. Trusted third-party binaries should be accompanied with installation instructions, or a link to relevant installation instructions.

To ensure data re-usabilty, the following standards are required when code is included in the data:

| Langauge | Standard |
| ------   | -------- |
| Python   | a `requirements.txt` containing the output of `pip freeze` |
| Julia    | both a `Project.toml` and a `Manifest.toml` |

If any code is written in a programming langauge not included in the table, the Data Steward should be consulted to define an appropriate standard.

**Q. Will your data be made freely available in the public domain to permit the widest re-use possible? Will your data be licensed using standard reuse licenses, in line with the obligations set out in the Grant Agreement?**

Data will be made freely available in the public domain via the TR and licensed under CC0 as stipulated in the GA.

**Q. Will the data produced in the project be useable by third parties, in particular after the end of the project?**

Data produced will never be removed from the TR by CFT PAN. Provided the TR exists, the data can be accessed by third parties. In the event that the TR is no longer available, the data will be migrated to an alternative trusted repository to ensure continued access and usability after the end of the project.

**Q. Will the provenance of the data be thoroughly documented using the appropriate standards?**

The provenance of the data can be traced via the versioning system of the TR.

**Q. Describe all relevant data quality assurance processes.**

Data must be reproducible as a condition of publication. As such, data generated must be accompanied by a self contained environment containing the scripts used to produce the data. These scripts must adhere to the requirements set out in this DMP. 

The Data Steward must have reviewed the data to confirm that it adheres to the DMP as a condition for publication of research using the data.

**Q. Further to the FAIR principles, DMPs should also address research outputs other than data, and should carefully consider aspects related to the allocation of resources, data security and ethical aspects.**

The project produces only numerical research data and no additional research outputs requiring separate management. Appropriate resources for storage, curation, and repository deposit are provided through the TR infrastructure. Data security is ensured by the repository's institutional hosting and backup procedures. No personal or sensitive data are involved, therefore, no specific ethical or privacy issues apply.

## 3. Other research outputs

**Q. In addition to the management of data, beneficiaries should also consider and plan for the management of other research outputs that may be generated or re-used throughout their projects. Such outputs can be either digital (e.g. software, workflows, protocols, models, etc.) or physical (e.g. new materials, antibodies, reagents, samples, etc.).**

The project does not produce research outputs other than numerical data, hence no additional digital or physical outputs requiring management will be generated.

**Q. Beneficiaries should consider which of the questions pertaining to FAIR data above, can apply to the management of other research outputs, and should strive to provide sufficient detail on how their research outputs will be managed and shared, or made available for re-use, in line with the FAIR principles.**

As no other research outputs are generated, the FAIR principles apply solely to the numerical data, which will be managed and shared via the TR in line with FAIR requirements.

## 4. Allocation of resources

**Q. What will the costs be for making data or other research outputs FAIR in your project (e.g. direct and indirect costs related to storage, archiving, re-use, security, etc.) ?**

Costs include (TBD):

1. Cost of 5'000 PLN gross/month to fund the 0.5 part-time salary of the Data Stewart for the duration of the project.

2. 10'000 EUR for the 10TiB of storage required for the project.

3. Estimated running costs of 4'000 EUR for electricity to host the server (5 years, current price list of energy in Poland). 

**Q. How will these be covered? Note that costs related to research data/output management are eligible as part of the Horizon Europe grant (if compliant with the Grant Agreement conditions)**

These costs will be covered by funds made available as part of the project grant.

**Q. Who will be responsible for data management in your project?**

The Data Steward will be responsible for management of data during the project. It is the responsibility of those who have generated the data to submit the data to the Data Steward as a condition for publishing any work that uses the data. No publications using data withheld from the Data Steward can proceed. This is to ensure the data adheres to the requirements of the DMP.  

**Q. How will long term preservation be ensured? Discuss the necessary resources to accomplish this (costs and potential value, who decides and how, what data will be kept and for how long)?**

The raw data, whose analysis has been used in publications, will be stored in accordance with the recommendations of the Polish Archive of New Records for 10 years after the project's completion. The metadata associated with this data will be preserved indefinitely to ensure readability and reusability.

## 5. Data security

**Q. What provisions are or will be in place for data security (including data recovery as well as secure storage/archiving and transfer of sensitive data)?**

All data is is open and freely available. No data is sensitive or personal. 

Data is backed up offline at CFT PAN in the LR. While the LR does not exist, data is instead backed up on the existing local-hosted Nextcloud server at CFT PAN: Nextcloud is an open-source cloud storage platform and includes a range of security features, such as encryption, secure servers, and data backup and recovery. Once the LR becomes operational, data shall be migrated to the LR. In the event the TR is no longer accessible. Data will be restored from the backup into a new trusted repository. 

**Q. Will the data be safely stored in trusted repositories for long term preservation and curation?**

The data will be stored on TR.

## 6. Ethics

**Q. Are there, or could there be, any ethics or legal issues that can have an impact on data sharing? These can also be discussed in the context of the ethics review. If relevant, include references to ethics deliverables and ethics chapter in the Description of the Action (DoA).**

Not applicable. 

**Q. Will informed consent for data sharing and long term preservation be included in questionnaires dealing with personal data?**

Not applicable.

## 7. Other issues

**Q. Do you, or will you, make use of other national/funder/sectorial/departmental procedures for data management? If yes, which ones (please list and briefly describe them)?**

The Polish regulations are to be introduced soon. For the time being CTP PAS is following the recommendations of Archive of New Records. According to the "Uniform List of Records" the data will be categorized as B category and therefore stored for 10 years.

| HISTORY OF CHANGES |  |  |
| ----- | ----- | ----- |
| VERSION | PUBLICATION  DATE | CHANGE |
| 0.1 | 04.03.2025 | Initial version (new MFF). |
| 0.2 | 18.03.2025 | Add more details about funds. Adjust sever size from 50 to 10 TiB in alignment of current plans. Remove Google Cloud Storage option as does not adhere to Fair. |
| 1.0 | 12.05.2025 | Clarify supported data formats and allow support for `.wdat`. Add standards for programming languages. Provide details of Nextcloud interim local repository. Other misc changes and typo fixes (see git diff). |
|  |  |  |

[^1]:  	*A qualified reference is a cross-reference that explains its intent. For example, X is regulator of Y is a much more qualified reference than X is associated with Y, or X see also Y. The goal therefore is to create as many meaningful links as possible between (meta)data resources to enrich the contextual knowledge about the data. (Source: [https://www.go-fair.org/fair-principles/i3-metadata-include-qualified-references-metadata/](https://www.go-fair.org/fair-principles/i3-metadata-include-qualified-references-metadata/))*

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAMAAAAolt3jAAADAFBMVEUAAAAAAAgAABMAAAcDADoAAD0EAFUPAGogGREiFHIxMGE/L6tFPR9JOz1JO05aT0xaVkxRTVRRTVZVT1dFQ2VOSW1cVm9eWXFeWnFfWnBeWXBIR3JGTZZjU0RkXm5mX2tmX21hYUZzdLWCdySXl4+UkZ6tkhuyrwGpoBm+txPVvQ7TtxDEtwDCqhzOrhLe2wbezg7uvwDp0gDq0gLozAXszgP/3wDz1gbowwD83w7/2QDn0wDsxgL/1wD/3gDrxh73ywD/3wH3xAD4xgD5xgD/0QD+zAD/0wD8xwD4xQD/zgD/1QDu0DXvyjLy5QD//wD18xTs6QLq4wD//wn//x3/9wPq5Af76wT//wb//wP/9gz//xL/9Ar/+wb//wX44wr/6wX//AD68gL//hD/7Q7/6gD/+gD/9AD/9A3/5Af/7AD/7QD/9QD/+QD//hL/5Qz/6AD/8AD/+AD/+QL//QX/4AD/6QD/5AD/5wP/5wD//y0AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABj1ZNiAAAAAXRSTlMAQObYZgAAAJdJREFUeF5jYMAC/PyhDGYQEcTM/P0DmMsCkmO+9cOU8R6IywQi/l26+/MdWBbI9eNkZWTiUlCCcp8wf+diZJJ/D+XqsgnJsLGLBAiBuX6s11j4JVlZv0sqgbivWFlYWdhYWcWcPgK5fixXWNhO3GRlZWWXBnI/svw1Z2Nl+3+ChcWbgYGRQfUjIyMb4w8GZrbfT8F2IwEAoosfhAm4YXkAAAAASUVORK5CYII=>
