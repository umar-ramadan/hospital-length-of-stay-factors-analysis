# Factors Associated with Hospital Length of Stay

### A Healthcare Data Analytics Project Using Python

## Project Overview

Length of stay (LOS) is an important indicator of hospital efficiency. Longer hospital stays can increase healthcare costs, occupy beds needed by other patients, and increase demands on healthcare staff.

This project analysed a synthetic dataset of 50,000 hospital admission records, created with Claude AI to resemble records from a Nigerian hospital. The objective was to investigate factors associated with hospital length of stay using Python, statistical testing, correlation analysis, effect-size analysis, and multiple linear regression.

The dataset contained data quality issues, including inconsistent spellings, missing values, impossible values, mixed date formats, and duplicate records. After cleaning, 48,019 records remained for analysis.

## Full Project Report

The detailed project report will be available here:

[View Full Hospital Length of Stay Analysis Report (PDF)](Hospital_Length_of_Stay_Factors_Analysis_Report.pdf)


**Dataset:** Synthetic hospital admission records  
**Records before cleaning:** 50,000  
**Records after cleaning:** 48,019  
**Tools:** Python, pandas, NumPy, SciPy, Matplotlib

## Project Objectives

- Assess and clean the quality of hospital admission data.
- Describe the distribution of hospital length of stay.
- Investigate factors associated with length of stay.
- Apply appropriate statistical tests to compare patient groups.
- Examine relationships using Pearson and Spearman correlation.
- Quantify effect sizes to support interpretation of findings.
- Build and evaluate a multiple linear regression model using log-transformed length of stay.

## Dataset Overview

The synthetic dataset was designed to resemble hospital admission records from a Nigerian healthcare setting.

The data included patient and admission characteristics, clinical information, ward, previous admissions, payment type, and 30-day readmission status.

The dataset was deliberately created with data quality problems to support practical data cleaning and validation.

## Tools and Technologies

- Python
- pandas
- NumPy
- SciPy
- Matplotlib
- Jupyter Notebook / Google Colab

## Data Cleaning

The data preparation process addressed several quality issues:

- Missing values
- Duplicate records
- Inconsistent spellings and category labels
- Impossible or invalid values
- Mixed date formats
- Data type standardisation

After cleaning, the dataset contained 48,019 records, compared with 50,000 records before cleaning.

## Statistical Methods

The project used several statistical techniques to investigate differences and relationships in length of stay:

- Descriptive statistics
- Independent-samples t-test
- Mann–Whitney U test
- One-way ANOVA
- Kruskal–Wallis test
- Pearson correlation
- Spearman rank correlation
- Effect-size analysis
- Multiple linear regression using log-transformed length of stay

The regression model was evaluated using a train–test split to assess its performance on unseen data.

## Key Findings

### Length of Stay

- Mean length of stay: 5.50 days
- Median length of stay: 4 days
- Observed range: 1–46 days

The difference between the mean and median suggests that the distribution of length of stay was influenced by patients with longer admissions.

### Factors Associated with Length of Stay

The analysis identified statistically significant associations between length of stay and:

- Primary diagnosis
- Comorbidity count
- Age
- Ward
- Previous admissions
- Admission type
- 30-day readmission status

Gender and payment type were not statistically significantly associated with length of stay in this analysis.

### Length of Stay by Diagnosis

Average length of stay varied across primary diagnoses:

| Primary Diagnosis | Average Length of Stay |
|---|---:|
| Tuberculosis | 7.98 days |
| Sepsis | 7.43 days |
| Stroke | 7.27 days |
| Gastroenteritis | 4.02 days |

Tuberculosis, sepsis, and stroke had the longest average stays among the diagnoses highlighted in the analysis, while gastroenteritis had a shorter average stay.

### Length of Stay by Ward

Patients admitted to the intensive care unit (ICU) stayed approximately 2.4 days longer, on average, than patients in the medical ward.

This is an observed difference in the synthetic dataset and should not be interpreted as evidence that ward placement causes longer stays.

## Regression Model Performance

A multiple linear regression model was developed using log-transformed length of stay.

- Test-set R²: 0.199
- The model explained approximately 19.9% of the variation in log-transformed length of stay in the test data.

The model achieved similar performance on the training and test data, suggesting that its performance was broadly consistent across the two datasets.

However, most of the variation in length of stay remained unexplained by the variables included in the model.

## Limitations

- The dataset is synthetic and does not represent verified real-world hospital records.
- The findings demonstrate associations, not causation.
- The analysis is limited to the variables available in the dataset.
- Statistical significance does not necessarily imply a large or practically important effect.
- The regression model explained only a portion of the variation in length of stay.

## Conclusion

This project demonstrated how Python can be used to clean healthcare data, investigate factors associated with hospital length of stay, conduct statistical tests, quantify effect sizes, and evaluate a regression model.

Diagnosis, comorbidity count, age, ward, previous admissions, admission type, and 30-day readmission status were associated with length of stay in the synthetic dataset.

The regression model explained approximately 19.9% of the variation in log-transformed length of stay on the test set, indicating that additional factors would be needed to explain more of the variation.

Because the dataset is synthetic, the findings should be treated as an analytical demonstration rather than clinical evidence.
