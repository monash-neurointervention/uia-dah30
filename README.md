# Days Alive and at Home at 30 Days (DAH30)

A simple, patient-centred way to measure recovery after treatment.

DAH30 is the number of days a patient is alive and at home in the first 30 days after treatment.

It combines survival, time in hospital, and recovery into a single, patient-centred outcome.

## WHY DAH30 MATTERS
Most medical outcomes focus on technical success or complications.

But for patients, an important question is often:  
*“How quickly will I get home and recover?”*

DAH30 answers this directly.

It reflects:
- Recovery after treatment
- Time spent in hospital
- Complications and readmissions
- Early survival

DAH30 aligns clinical outcomes with what matters most to patients: *time at home.*

DAH30 is already used in surgery and healthcare systems and is designed for real-world data and clinical registries.

## HOW DAH30 IS DEFINED

### Core Definition
DAH30 = Number of days alive and at home within 30 days after treatment

### How it is calculated
Start with 30 days, then subtract:
- Days in hospital after treatment
- Days in rehabilitation
- Days from unplanned readmissions
Death within 30 days means DAH30 = 0.

### Key rules
- Day 0 is the date of treatment (days before treatment are not included)
- Patient death within 30-days means DAH30 = 0
- Unplanned re-admissions DO reduce DAH30
- Planned readmissions (e.g. staged procedures) DO NOT reduce DAH30
- Emergency department visits without admission DO NOT reduce DAH30

### Simple Formula
DAH30 = 30 − (hospital days + rehab days + unplanned readmission days)

### SIMPLE EXAMPLES
Example 1 (Straightforward recovery)
- Hospital stay: 2 days
- No readmissions
- DAH30 = 28 days 

Example 2 (Complication + readmission)
- Hospital stay: 5 days
- Readmission: 5 days
- DAH30 = 20 days

Example 3 (Planned second procedure)
- Hospital stay: 2 days
- Planned readmission later
- DAH30 = 28 days (planned care does not reduce DAH30)

### QUICK START (FOR RESEARCHERS)

Use the following formatted excel sheet and practice running through this rmarkdown document.  
[minimum_dataset.xlsx](minimum_dataset.xlsx)  
[workbook_minimum.Rmd](workbook_minimum.Rmd)  

The code should create the following output file in your working directory with calculated DAH30 scores.  
[30days.xlsx](30days.xlsx)

If the above steps work for you, you can try editing the minimum_dataset to include your own data with the same formatting.  
For interrogatability, the output 30days.xlsx will show you which date intervals have been subtracted from the 30 post-op days under the column "merged_intervals", as well as counts for those days under "overlap_days".

### WHAT OUR RESEARCH SHOWS

DAH30 has been evaluated in 614 unruptured brain aneurysm treatments at a major neurovascular centre in Melbourne (Monash Health).
- The typical patient spent 27 out of 30 days at home after treatment
- Most patients were discharged home quickly and remained at home
- Patients undergoing endovascular treatment spent more time at home than those undergoing surgery, reflecting the less invasive nature and faster recovery
- Longer or more complex procedures were associated with slower recovery
- Patient factors such as frailty and overall health also influenced time at home

Overall, DAH30 provides a simple and reliable way to measure real-world recovery after unruptured brain aneurysm treatment.

### REFERENCE
Chandra RV, Taylor F, Gall S, et al.  
30-day home time as a patient-centered outcome after treatment of unruptured intracranial aneurysms  
J NeuroInterventional Surgery, 2026  
[https://doi.org/10.1136/jnis-2025-024914](https://doi.org/10.1136/jnis-2025-024914)

### WHY THIS METRIC IS USEFUL
For patients
- Clear understanding of recovery
- Helps guide expectations

For clinicians
- Simple and objective
- Reflects real recovery, not just technical success

For researchers and systems
- Can be calculated from administrative data
- Suitable for registries and large datasets
- Reduces bias compared to patient-reported outcomes 

### [COLLABORATION](https://monash-neurointervention.github.io/collaboration)
