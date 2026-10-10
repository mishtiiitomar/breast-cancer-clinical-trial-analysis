# Breast Cancer Clinical Trial Outcomes Analysis

### Exploratory Data Analysis Using Python and SQL

## Project Overview

This project examines clinical trial completion and termination patterns in breast cancer research using publicly available data from ClinicalTrials.gov.

The analysis explores relationships between clinical trial outcomes and characteristics such as trial phase, patient enrollment, funding source, and study duration.

**Dataset:** 1,528 interventional breast cancer clinical trials  
**Study Start Period:** 2015–2023  
**Data Source:** ClinicalTrials.gov  
**Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, SQLite, Google Colab

## Research Questions

1. How do observed termination proportions differ across clinical trial phases?
2. How does patient enrollment compare between completed and terminated trials?
3. Are funding categories associated with different termination patterns?
4. How does reported trial duration differ by outcome?
5. How do observed termination proportions vary across study-start years?

## Key Findings

**1. Clinical Trial Outcomes**

Of the 1,528 studies analyzed, 1,091 were completed (71.4%), while 437 were terminated (28.6%).

**2. Trial Phase**

Combined Phase 1/2 trials had the highest observed termination proportion (41.0%), followed by Phase 2 trials (31.8%). Phase 4 studies had the lowest observed proportion (13.0%).

**3. Patient Enrollment**

Completed trials had a median enrollment of 54 participants, compared with 20 for terminated studies. The enrollment distribution was right-skewed, so median values and log-transformed visualizations were used to support comparisons.

**4. Funding Source**

Industry-funded studies had an observed termination proportion of 33.1%, compared with 24.8% for studies categorized as Other.

**5. Trial Duration**

Completed trials had a median reported duration of 1,221 days, compared with 1,004 days for terminated studies.

## Methodology

- Imported and explored publicly available clinical trial records.
- Cleaned categorical variables and standardized date fields.
- Used Pandas for aggregation and descriptive analysis.
- Applied SQLite queries to summarize trial characteristics.
- Created bar charts, box plots, histograms, and temporal visualizations.
- Interpreted relationships while considering potential selection bias and confounding factors.

## Repository Contents

- `clinical_trial_analysis.ipynb` — Complete Python and SQL notebook with visualizations and findings.
- `ctg-studies.csv` — ClinicalTrials.gov data used for the analysis.
- `README.md` — Project overview, methodology, and key findings.

## How to Run

1. Download the notebook and CSV file from this repository.
2. Open the notebook in Google Colab.
3. Upload `ctg-studies.csv` to the Colab session.
4. Run the notebook cells in order.

## Limitations

This dataset includes only completed and terminated interventional breast cancer studies, rather than all registered trials. The observed termination proportions should not be interpreted as overall clinical trial failure probabilities.

Differences in trial phase, enrollment, funding, and duration are descriptive associations and do not establish causation. Enrollment may be affected by early termination, and some reported dates may be approximate.

The study-start-year comparisons may be affected by selection bias because ongoing trials were excluded.

## Conclusion

This project demonstrates how Python and SQL can be used to explore operational patterns in clinical research data.

The analysis identified differences in termination proportions, patient enrollment, and study duration across trial characteristics. These findings provide a foundation for further investigation into clinical trial operations and research outcomes.

*Data Source: [ClinicalTrials.gov](https://clinicaltrials.gov/)*
