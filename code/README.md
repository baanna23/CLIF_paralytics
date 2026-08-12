 ## Code directory

This directory contains scripts for the CLIF_paralytics project workflow. The general workflow consists of two main steps: cohort identification and analysis. 

### General Workflow

1. Add site details into config_template file and save as config.json in config folder

2. Run the cohort_identification script (00)
   This script will:
   - Apply inclusion and exclusion criteria
   - Select required fields from each table
   - Filter tables to include only required observations

   Expected outputs:
   - cohort_ids: a list of unique identifiers for the study cohort DO NOT SHARE, includes PHI
   - cohort_data: the filtered study cohort data; project_tables folder DO NOT SHARE, includes PHI
   
2. Run the 01 script after completing 00. This script contains the main analysis code for the project.

   Input: cleaned_cohort_data from 00 file Step 1 above. 

   Output: Tables and figures, collected in project_output_UPLOAD folder as individual files (Tables and figures). The total number depends on site configurations (# of hospitals, # of study periods)

3. Run to 02 script after receiving instructions from primary site. This script utilizes a csv file of global estimates derived from local estimates provided by each site to the primary site. 


