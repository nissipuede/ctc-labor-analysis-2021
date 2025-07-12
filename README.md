# 2024-2025 Final Project (PPOL6903 - Data Science for Public Policy): Did the 2021 Child Tax Credit Affect Labor Supply?

This repository contains a Jupyter Notebook and accompanying white paper for my final project in **PPOL6903: Data Science for Public Policy** at Georgetown University. The project investigates whether the refundable portion of the expanded 2021 Child Tax Credit (CTC) impacted labor supply using CPS microdata and machine learning methods.

## Research Summary

- **Research Question**: Did the refundable 2021 CTC (i.e., the Additional Child Tax Credit or ACTC) influence weekly hours worked among U.S. households?
- **Approach**: I use microdata from the 2022 CPS ASEC (reflecting 2021 data) to estimate a linear regression model and a decision tree classifier.
- **Outcome**: Weekly hours worked (continuous variable), as well as binned labor supply groups.
- **Treatment**: Receipt and amount of the ACTC, alongside key covariates.
- **Result**:
  - **Linear Regression**: Minimal average effect of ACTC amount on hours worked.
  - **Decision Tree Classifier**: Identifies age, EITC, and ACTC as important features, achieving ~78% test accuracy.

## Data Scope

- **Source**: IPUMS Current Population Survey (CPS) Annual Social and Economic Supplement (ASEC)
- **Period**: 2021 (data collected in 2022 ASEC)
- **Sample**: 73,713 individuals aged 18–85 with non-zero employment
- **Target Variable**: Weekly hours worked (`UHRSWORKLY`)
- **Key Predictors**: 
  - ACTC amount and receipt
  - EITC amount
  - Age
  - Health status
  - Disability-related work limitations

## Repository Structure

| File Name                                  | Description                                   |
|--------------------------------------------|-----------------------------------------------|
| `PPOL6903 - Final Project_nc809.html`      | Jupyter Notebook (Python 3.9) |
| `PPOL6803 - Final Project - White Paper.pdf` | Policy paper summarizing the methods and findings |
| *(No data files included)*                 | Source data omitted due to licensing/size     |

## Note on Data Availability

All data are derived from the **IPUMS CPS ASEC** microdata, which is publicly accessible. The raw or cleaned data files are not included in this repository due to size and licensing constraints.

🔗 Access CPS ASEC datasets here:  
https://cps.ipums.org/cps-action/data/download

## Methods Summary

- **Software**: Python 3.9 (Jupyter Notebook)
- **Techniques**:
  - Linear Regression
  - Decision Tree Classification
- **Data Prep**: Feature selection, dummy variables, and binning of target variable
- **Evaluation**:
  - R² scores for regression
  - Accuracy, validation curves, and learning curves for decision tree

## Author

**Nissi Cantu**  
Master of Public Policy & Master of Business Administration  
Georgetown University  
📧 nc809@georgetown.edu  
🔗 [LinkedIn](https://www.linkedin.com/in/nissi-cantu/)
