# PCORnet Diagnostic Query Package

### Purpose
This code package evaluates a DataMart's conformance to the PCORnet Common Data Model (CDM) v3.0 SAS table structure, variable names, variable lengths, and data types.  

The Diagnostic Query Package is a complement to the [Data Characterization Query Package] (https://github.com/PCORnet-DRN-OC/PCORnet-Data-Characterization). The Diagnostic Query is run **first**, prior to Data Characterization.

### PCORnet data partners run code packages distributed through PopMedNet
It's crucially important for data partners to follow the process of running the exact code module distributed to your DataMart by the Operations Center (via PopMedNet). This process ensures that end-to-end provenance is preserved. Complete instructions on how to run this code are provided to PCORnet DataMarts when the query is distributed to a given DataMart. 

### This GitHub repository is a copy for reference
PCORnet's Distributed Research Network Operations Center (DRN OC) is responsible for distribution of the production code package to data partners, which happens within PopMedNet.

Waves of data partner querying may result in more than one code package being active at any given time. Beta testing is also an important ongoing activity.

Therefore, **this repository is not the production version of the code package**, but instead serves as a copy for reference and knowledge sharing.

### System Requirements
This code is designed to run in SAS versions 9.3 or higher. No other SAS packages are necessary. 

### Scope
This query examines all 15 tables and all fields except the RAW fields. As noted in the PCORnet CDM specification, all tables must be present in an instantiation of the CDM, even if the table does not contain any records. The DEMOGRAPHIC, ENROLLMENT, ENCOUNTER, DIAGNOSIS, PROCEDURES, VITAL, and HARVEST tables are expected to be populated by all CDRNs. 

CDM specifications are available at [http://www.pcornet.org/pcornet-common-data-model/] (http://www.pcornet.org/pcornet-common-data-model/). This version of the query allows DataMarts to incorporate [CDM errata] (https://github.com/CDMFORUM/CDM-ERRATA) identified as of January 20, 2016.

### Acknowledgments
This code package was developed by the Data Characterization Development Team in the DRN OC, with members from the Duke Clinical Research Institute. We gratefully acknowledge their work and individual contributions.
