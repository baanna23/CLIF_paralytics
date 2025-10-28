# Paralytic use across CLIF consortium*

## CLIF VERSION 

2.1

## Objective

To describe variability in paralytic use across the CLIF consortium with a focus on patients who meet ROSE trial hypoxemia criteria. 

## Required CLIF tables and fields

Example:
The following tables are required:
1. **patient**: `patient_id`, `race_category`, `ethnicity_category`, `sex_category`
2. **hospitalization**: `patient_id`, `hospitalization_id`, `admission_dttm`, `discharge_dttm`, `age_at_admission`
3. **vitals**: `hospitalization_id`, `recorded_dttm`, `vital_category`, `vital_value`
   - `vital_category` = 'heart_rate', 'resp_rate', 'map', 'resp_rate', 'spo2'
4. **labs**: `hospitalization_id`, `lab_result_dttm`, `lab_category`, `lab_value`
   - `lab_category` = 'lactate, ph_arterial, ph_venous, bilirubin, creatinine, po2_arterial'
5. **medication_admin_continuous**: `hospitalization_id`, `admin_dttm`, `med_name`, `med_category`, `med_dose`, `med_dose_unit`
   - `med_category` = "norepinephrine", "epinephrine", "phenylephrine", "vasopressin", "dopamine", "angiotensin", "cisatracurium", "vecuronium", "rocuronium"
6. **medication_admin_intermittent**: `hospitalization_id`, `admin_dttm`, `med_name`, `med_category`, `med_dose`, `med_dose_unit`
   - `med_category` = "cisatracurium", "vecuronium", "rocuronium", "succinylcholine"
7. **respiratory_support**: `hospitalization_id`, `recorded_dttm`, `device_category`, `mode_category`, `tracheostomy`, `fio2_set`, `lpm_set`, `resp_rate_set`, `peep_set`, `resp_rate_obs`, 'peak_inspiratory_pressure_obs', 'minute_vent_obs', 'plateau_pressure_obs'

## Cohort identification
Patients on invasive mechanical ventilation, with primary outcome cohort restricted to patients who meet criteria based on ROSE RCT inclusion and exclusion criteria: No chronic mechanical ventilation (trach within 24h of intubation), PEEP >=8, P/F (or equivalent S/F x2) <=150. Excludes patients who transfer from hospital outside of health system while already receiving IMV. 

## Expected Results
18 csv files and 9 pdf figures, saves in project_output folder (in path input by site PI at beginning of 01 file)

## Detailed Instructions for running the project

Detailed instructions on the code workflow are provided in the [code directory](code/README.md)

** NOTE: For this project, there is no config file to update. Provide your time zone and paths to local data directly in the 00 and 01 files. 

---


