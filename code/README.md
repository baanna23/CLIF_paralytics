 ## Code directory

This directory contains scripts for the CLIF_paralytics project workflow. The general workflow consists of two main steps: cohort identification and analysis. 

### General Workflow

1. Run the cohort_identification script (00)
   This script will:
   - Apply inclusion and exclusion criteria
   - Select required fields from each table
   - Filter tables to include only required observations

   Expected outputs:
   - cohort_ids: a list of unique identifiers for the study cohort
   - cohort_data: the filtered study cohort data; project_tables folder DO NOT SHARE, includes PHI
   
2. Run the analysis script (01)
   This script contains the main analysis code for the project.

   Input: cleaned_cohort_data from 00 file Step 1 above. 

   Output: Tables and figures, collected in project_output folder as individual files (Tables) and in graphs folder (figure)


