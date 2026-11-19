### Overview  
This repository contains select code to identify Medicaid and Medicare behavioral health service use, including  
  
- Emergency department (ED) visits  
- Inpatient days  
- In-person outpatient visits  
- Telehealth visits  
- Residential treatment days  

among dual eligible enrollees with diagnoses of:  

- Mild or moderate mental illness  
- Serious mental illness  
- Substance use disorder  

as published in: Kim H, Edelstein S, Senders A, et al. Medicare and Medicaid Behavioral Health Service Use Among Dual-Eligible Special Needs Plan Enrollees. JAMA Netw Open. 2026;9(1):e2554246. doi:10.1001/jamanetworkopen.2025.54246


### Data availability  
These analyses use CMS Research Identifiable Files (RIFs) obtained under a Data Use Agreement with CMS. The data cannot be redistributed and are not included in this repository. Researchers may [request RIF access through CMS](https://www.cms.gov/data-research/cms-data/data-available-researchers). 

The following source files were used in this study:  

- 2021 [Medicare Master Beneficiary Summary File Base A/B/C/D](https://resdac.org/cms-data/files/mbsf-base) 
- 2021 [Medicare Encounter Inpatient](https://resdac.org/cms-data/files/ip-encounter)
- 2021 [Medicare Encounter Outpatient](https://resdac.org/cms-data/files/op-encounter)
- 2021 [Medicare Encounter Carrier](https://resdac.org/cms-data/files/carrier-encounter)
- 2021 [Medicare Encounter Skilled Nursing Facility](https://resdac.org/cms-data/files/snf-encounter)
- 2021 [Medicare Encounter Home Health Agency](https://resdac.org/cms-data/files/hha-encounter)
- 2021 [T-MSIS Analytic File Demographic and Eligibility](https://resdac.org/cms-data/files/taf-de)  
- 2021 [T-MSIS Analytic File Other Services](https://resdac.org/cms-data/files/taf-ot)  
- 2021 [T-MSIS Analytic File Inpatient](https://resdac.org/cms-data/files/taf-ip)  
- 2021 [T-MSIS Analytic File Long Term Care](https://resdac.org/cms-data/files/taf-lt)  
  
  
### Scope and intended use
This is not a turnkey pipeline; the code is excerpted from a larger analytic workflow and omits data acquisition, cohort construction, cleaning, and validation steps. It assumes the user has already built an analytic cohort file at the enrollee-month level. Users will need to adapt any file paths, variable names, and data structures to their own environment.  
  
  
### Included scripts 
This repo includes the following scripts:  
  
- select_code_to_identify_MH_conditions.Rmd  
- select_code_to_identify_SUD.Rmd  
- select_code_to_identify_ed_visits.Rmd  
- select_code_to_identify_outpatient_visits.Rmd  
- select_code_to_identify_ip_residential_days.Rmd  
  
  
### Included look-up tables  
This repo includes the following look-up tables:  

- sud_codes.Rdata  
- mental_health_icd_codes.csv  
- milbank_ip_residential_codes.csv  
- outpt_bh_cpts.csv  