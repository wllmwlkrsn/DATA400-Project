# DATA400-Project

The purpose of this project is to improve our understanding of lung adenocarcinoma (LUAD), particularly with respect to patient survival and treatment regimen, by determining distinct patient groups as well as predicting survival of LUAD patients based on exome sequencing of their tumor. The datasets used in this project are taken from published studies that are available on [cBioPortal](https://www.cbioportal.org/), [Cancer Hotspots](https://www.cancerhotspots.org/#/home), and [DepMap](https://depmap.org/portal/home/#/) -- this tool was used to validate the list of LUAD cancer cell lines.

[cBioPortal](https://www.cbioportal.org/) Studies/Data included:
* Cancer Cell Line Encyclopedia ([Broad, 2019](https://pubmed.ncbi.nlm.nih.gov/31068700/))
* Metastatic Non-Small Cell Lung Cancer ([MSK, Nature Medicine 2022](https://pubmed.ncbi.nlm.nih.gov/36357680/))
* Lung Adenocarcinoma Met Organotropism ([MSK, Cancer Cell 2023](https://pubmed.ncbi.nlm.nih.gov/37084736/))

Mutation, clinical, and sample datasets were used from these studies.

[Cancer Hotspots](https://www.cancerhotspots.org/#/home) Studies/Data included:
* V2 Mutational Data ([Chang et al. 2017](https://pubmed.ncbi.nlm.nih.gov/29247016/))

The data from the [Cancer Hotspots](https://www.cancerhotspots.org/#/home) was used filter out non-oncogenic mutations. 

The processed data for this project includes:   
`PATIENT_ID`: A unique ID of each patient.   
`CURRENT_AGE:` The patient's age at the time of sequencing, in years.   
`SEX:` The sex of the patient.   
`OS_STATUS:` The status (alive/dead) of the patient at a specific timepoint.  
`OS_MONTHS:`  Time, in months, from diagnosis of the patient.  
`RACE:` The race of the patient.  
`ETHNICITY:` The ethnicity of the patient.  
`SMOKING_STATUS:` True/Ever: Patient is a smoker or formerly smoked. False/Never: Patient has never smoked.  
`Tumor_Sample_Barcode:` Unique ID of each sample.  
`HAD_SURGERY:` Whether the patient recieved surgery to remove tumor(s). Not complete across all datasets. We are currently working to combine this variable across all datasets.  
`Binary mutational hotspot variables:` Binary variables which indicate whether patient's tumor contains a mutation at each of the 1,165 mutational hotspots identified by [Cancer Hotspots](https://www.cancerhotspots.org/#/home).

