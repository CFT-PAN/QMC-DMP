*(To be filled in and uploaded as deliverable in the Portal Grant Management System, at the due date foreseen in the system (and regularly updated).*

![Picture 1][image1]*The template is recommended but not mandatory. If you do not use it, please make however sure that you comply with the research data management requirements under Article 17 of the Grant Agreement.)*

| PROJECT |  |
| :---- | :---- |
| **Project number:** | \[project number\] |
| **Project acronym:** | **EUCENTRAL** |
| **Project name:** | \[project title\] |

| DATA MANAGEMENT PLAN |  |
| :---- | :---- |
| **Date**: | \[18/04/2025\] |
| **Version:** | \[0.2\] |

## **Glossary of terms:**

1. **TR:** The Trusted Repository. In this case the Zenodo repository.

2. **CR:** The Code Repository. In this case, Github.

3. **DMP:** This Data Management Plan

4. **GA:** The Grant Agreement. 

1. ## **Data Summary**

*Will you re-use any existing data and what will you re-use it for? State the reasons if re-use of any existing data has been considered but discarded.* 

**No existing data will be reused.**

*What types and formats of data will the project generate or re-use?*

**The project will generate representations of a quantum mechanical wave-functions stored as HDF5. Input parameters will be stored as plain text JSON (.json). In the event HDF5 and JSON are unsuitable, open-source formats. Such formats must be accompanied by an open-source with details (included version, required packages) of a language environment that can load such a format.** 

**Figures generated from the data sill be exported as both a printable image format (.png) and the scalable vector graphics format (.pdf).** 

*What is the purpose of the data generation or re-use and its relation to the objectives of the project?*

**The data is as result of numerical simulations of quantum mechanical systems. The purpose of the data is such that it can be used to provide insights into the quantum many-body problem. Such insights can then be used to a) inform experiment and b) advance theoretical understanding. Specifically, data will be used in publication of peer-reviewed research articles.** 

*What is the expected size of the data that you intend to generate or re-use?*

**Across the 5 year project, the total size of the data generated is expected to be no more than 10TiB.** 

*What is the origin/provenance of the data, either generated or re-used?*

**All data is generated as both input and output of numerical simulations.**

*To whom might your data be useful ('data utility'), outside your project?*

**The data will be useful to researchers who wish to perform further analysis on the outputs of the data.**

2. ## **FAIR data**

   1. ### **Making data findable, including provisions for metadata**

*Will data be identified by a persistent identifier?*

**Data will be assigned a DOI by the TR. Code will be not be assigned a DOI by default as the CR does not assign DOI. Instead, the CR repository name forms the unique identifier for codebases stored at the CR. This is such that code can be published in journals where a DOI gets assigned by the journals.** 

*Will rich metadata be provided to allow discovery? What metadata will be created? What disciplinary or general standards will be followed? In case metadata standards do not exist in your discipline, please outline what type of metadata will be created and how.*

**Metadata will adhere to the Dublin Core (DCMT) standard.** 

*Will search keywords be provided in the metadata to optimize the possibility for discovery and then potential re-use?*

**Keywords will be used when required by publications associated with the data. When required by publication, there will be a one-to-one correspondence between the data keywords and the publication keywords.**

*Will metadata be offered in such a way that it can be harvested and indexed?* 

***“*****All metadata is exported via OAI-PMH and can be harvested” as per the TR policy.**

2. ### **Making data accessible**

***Repository:***

*Will the data be deposited in a trusted repository?*

**Data will be stored in the TR. The TR is hosted and managed by CERN which have experience handling operating large data repositories. The CERN project has funding for the next 20 years and the TR will exist for along as the CERN project had funding.** 

**Code will be stored publicly in the CR. The CR is the most widely used repository for code storage and version control and is already routinely used by many researchers.**  

*Have you explored appropriate arrangements with the identified repository where your data will be deposited?* 

**Not applicable as the TR and the CR are free to use by the public.**

*Does the repository ensure that the data is assigned an identifier? Will the repository resolve the identifier to a digital object?* 

**The TR assigns a DOI to each set of data, which will be used as the identifier. Furthermore, the TR allows versioning of data.** 

***Data:***

*Will all data be made openly available? If certain datasets cannot be shared (or need to be shared under restricted access conditions), explain why, clearly separating legal and contractual reasons from intentional restrictions. Note that in multi-beneficiary projects it is also possible for specific beneficiaries to keep their data closed if opening their data goes against their legitimate interests or other constraints as per the Grant Agreement.*

**All data used in publication will be made openly available.** 

*If an embargo is applied to give time to publish or seek protection of the intellectual property (e.g. patents), specify why and how long this will apply, bearing in mind that research data should be made available as soon as possible.*

**Not applicable.**

*Will the data be accessible through a free and standardized access protocol?*

**According to TR policy, “access to metadata and data files is provided over standard protocols such as HTTP and OAI-PMH”.**

*If there are restrictions on use, how will access be provided to the data, both during and after the end of the project?*

**There are no restrictions on the use of the data.**

*How will the identity of the person accessing the data be ascertained?*

**Not applicable.**

*Is there a need for a data access committee (e.g. to evaluate/approve access requests to personal/sensitive data)?*

**As data is not sensitive or personal, all requests will be granted by the Data Steward automatically.** 

***Metadata:***

*Will metadata be made openly available and licenced under a public domain dedication CC0, as per the Grant Agreement? If not, please clarify why. Will metadata contain information to enable the user to access the data?* 

**Yes data will be licensed under CC0 as per both the GA and the TR policy and is openly available.**

*How long will the data remain available and findable? Will metadata be guaranteed to remain available after data is no longer available?*

**Data and accompanying metadata will be made available for as long as it can be hosted at the TR. Data will also be backed at CFT-PAN offline for the duration of the project plus an additional 5 years at a minimum, At the end of period, an assessment of the current data storage capabilities by the Data Steward will take place to evaluate for how long the data can be stored going forward.**

*Will documentation or reference about any software be needed to access or read the data be included? Will it be possible to include the relevant software (e.g. in open source code)?*

**All data will be fully reproducible via scripts included in the repository, with an accompanying readme on how to do so. Any code required by the data developed as part of the Project, is hosted at an accompanying open-source code base repository at the CR.**

3. ### **Making data interoperable**

*What data and metadata vocabularies, standards, formats or methodologies will you follow to make your data interoperable to allow data exchange and re-use within and across disciplines? Will you follow community-endorsed interoperability best practices? Which ones?* 

**Data will be stored as HDF5 (.h5, .hdf5). HDF5 is standard data storage format for heterogeneous data readable by a wide variety of different software and programming languages. Input parameters must be stored as human-readable JSON (.json). Metadata will adhere to Dublin Core standard.** 

*In case it is unavoidable that you use uncommon or generate project specific ontologies or vocabularies, will you provide mappings to more commonly used ontologies? Will you openly publish the generated ontologies or vocabularies to allow reusing, refining or extending them?*

**All mappings will be published and included in the data repository.** 

*Will your data include qualified references[^1] to other data (e.g. other data from your project, or datasets from previous research)?*

**Qualified references will be used where appropriate.**

4. ### **Increase data re-use**

*How will you provide documentation needed to validate data analysis and facilitate data re-use (e.g. readme files with information on methodology, codebooks, data cleaning, analyses, variable definitions, units of measurement, etc.)?*

**All data used in publication must be reproducible as a requirement for publication. Data reproducibility is ensured by:**

1. **Any physical variables appearing in data and data-generating code must be accompanied with physical units as a code comment. All non-derivative (input) variables must be accompanied by a code comment explaining their function.** 

2. **A source code (non-binary) script must be included in the data repository that can reproduce the data.** 

3. **Any binary files produced and required to produce the data must be accompanied with the source code and details on how the binary can be generated. Trusted third-party binaries should be accompanied with installation instructions, or a link to relevant installation instructions.** 

*Will your data be made freely available in the public domain to permit the widest re-use possible? Will your data be licensed using standard reuse licenses, in line with the obligations set out in the Grant Agreement?*

**Data will be made freely available in the public domain via the TR and licensed under CC0 as stipulated in the GA.**

*Will the data produced in the project be useable by third parties, in particular after the end of the project?*

**Data produced will never be removed from the TR by CFT. Provided the TR exists data can be accessed by third-parties. In the event the TR is no longer available,** 

*Will the provenance of the data be thoroughly documented using the appropriate standards?*

**The provenance of the data can be traced via the versioning system of the TR.**

*Describe all relevant data quality assurance processes.*

**Data must be reproducible as a condition of publication. As such, data generated must be accompanied by a self contained environment containing the scripts used to produce the data. These scripts must adhere to the requirements set out in this DMP.** 

**The Data Steward must have reviewed the data to confirm that it adheres to the DMP as a condition for publication of research using the data/** 

*Further to the FAIR principles, DMPs should also address research outputs other than data, and should carefully consider aspects related to the allocation of resources, data security and ethical aspects.*

3. ## **Other research outputs**

*In addition to the management of data, beneficiaries should also consider and plan for the management of other research outputs that may be generated or re-used throughout their projects. Such outputs can be either digital (e.g. software, workflows, protocols, models, etc.) or physical (e.g. new materials, antibodies, reagents, samples, etc.).*

**Such outputs have been considered by the DMP**

*Beneficiaries should consider which of the questions pertaining to FAIR data above, can apply to the management of other research outputs, and should strive to provide sufficient detail on how their research outputs will be managed and shared, or made available for re-use, in line with the FAIR principles.*

4. ## **Allocation of resources**

*What will the costs be for making data or other research outputs FAIR in your project (e.g. direct and indirect costs related to storage, archiving, re-use, security, etc.) ?*

**Costs include (TBD):**

1. **Salary XXXX of the Data Stewart for the duration of the project.**

4. **10,000 euro for the 10TiB of storage required for the project.**

5. **Estimated running costs of 4 000 euro for electricity to host the server (5 years, current price list of energy in Poland).** 

*How will these be covered? Note that costs related to research data/output management are eligible as part of the Horizon Europe grant (if compliant with the Grant Agreement conditions)*

**These costs will be covered by funds made available as part of the project grant.**

*Who will be responsible for data management in your project?*

**The Data Steward will be responsible for management of data during the project. It is the responsibility of those who have generated the data to submit the data to the Data Steward as a condition for publishing any work that uses the data. No publications using data withheld from the Data Steward can proceed. This is to ensure the data adheres to the requirements of the DMP.**  

*How will long term preservation be ensured? Discuss the necessary resources to accomplish this (costs and potential value, who decides and how, what data will be kept and for how long)?*

**The raw data, whose analysis has been used in publications, will be stored in accordance with the recommendations of the Polish Archive of New Records for 10 years after the project's completion. The metadata associated with this data will be preserved indefinitely to ensure readability and reusability.**

5. ## **Data security**

*What provisions are or will be in place for data security (including data recovery as well as secure storage/archiving and transfer of sensitive data)?*

**All data is is open and freely available. No data is sensitive or personal.** 

**Data is backed up offline at CFT and online at Google Cloud. In the event the TR is no longer accessible. Data will be restored from the backup into a new trusted repository.** 

*Will the data be safely stored in trusted repositories for long term preservation and curation?*

**The data will be stored on at TR.**

6. ## **Ethics**

*Are there, or could there be, any ethics or legal issues that can have an impact on data sharing? These can also be discussed in the context of the ethics review. If relevant, include references to ethics deliverables and ethics chapter in the Description of the Action (DoA).*

**Not applicable.** 

*Will informed consent for data sharing and long term preservation be included in questionnaires dealing with personal data?*

**Not applicable.**

7. ## **Other issues**

*Do you, or will you, make use of other national/funder/sectorial/departmental procedures for data management? If yes, which ones (please list and briefly describe them)?*

**The Polish regulations are to be introduced soon. For the time being CTP PAS is following the recommendations of Archive of New Records. According to the "Uniform List of Records" the data will be categorized as B category and therefore stored for 10 years.**

| HISTORY OF CHANGES |  |  |
| ----- | ----- | ----- |
| VERSION | PUBLICATION  DATE | CHANGE |
| 0.1 | 04.03.2025 | Initial version (new MFF). |
| 0.2 | 18.03.2025 | Add more details about funds. Adjust sever size from 50 to 10 TiB in alignment of current plans. Remove Google Cloud Storage option as does not adhere to Fair. |
|  |  |  |
|  |  |  |

[^1]:  	*A qualified reference is a cross-reference that explains its intent. For example, X is regulator of Y is a much more qualified reference than X is associated with Y, or X see also Y. The goal therefore is to create as many meaningful links as possible between (meta)data resources to enrich the contextual knowledge about the data. (Source: [https://www.go-fair.org/fair-principles/i3-metadata-include-qualified-references-metadata/](https://www.go-fair.org/fair-principles/i3-metadata-include-qualified-references-metadata/))*

[image1]: <data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAAOCAMAAAAolt3jAAADAFBMVEUAAAAAAAgAABMAAAcDADoAAD0EAFUPAGogGREiFHIxMGE/L6tFPR9JOz1JO05aT0xaVkxRTVRRTVZVT1dFQ2VOSW1cVm9eWXFeWnFfWnBeWXBIR3JGTZZjU0RkXm5mX2tmX21hYUZzdLWCdySXl4+UkZ6tkhuyrwGpoBm+txPVvQ7TtxDEtwDCqhzOrhLe2wbezg7uvwDp0gDq0gLozAXszgP/3wDz1gbowwD83w7/2QDn0wDsxgL/1wD/3gDrxh73ywD/3wH3xAD4xgD5xgD/0QD+zAD/0wD8xwD4xQD/zgD/1QDu0DXvyjLy5QD//wD18xTs6QLq4wD//wn//x3/9wPq5Af76wT//wb//wP/9gz//xL/9Ar/+wb//wX44wr/6wX//AD68gL//hD/7Q7/6gD/+gD/9AD/9A3/5Af/7AD/7QD/9QD/+QD//hL/5Qz/6AD/8AD/+AD/+QL//QX/4AD/6QD/5AD/5wP/5wD//y0AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABj1ZNiAAAAAXRSTlMAQObYZgAAAJdJREFUeF5jYMAC/PyhDGYQEcTM/P0DmMsCkmO+9cOU8R6IywQi/l26+/MdWBbI9eNkZWTiUlCCcp8wf+diZJJ/D+XqsgnJsLGLBAiBuX6s11j4JVlZv0sqgbivWFlYWdhYWcWcPgK5fixXWNhO3GRlZWWXBnI/svw1Z2Nl+3+ChcWbgYGRQfUjIyMb4w8GZrbfT8F2IwEAoosfhAm4YXkAAAAASUVORK5CYII=>