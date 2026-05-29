# **BMI CATEGORY, BLOOD PRESSURE,AND  THEIR ASSOCIATION IN SCHOOL-AGED(6-19 YEARS) CHILDREN: A COMPARATIVE ANALYSIS OF UTURU,ABIA STATE ,NIGERIA AND NHANES USING WHO STANDARDS**
## DESCRIPTION
This project analyzes the relationship between BMI categories and blood pressure in school-aged children in uturu,Abia State , Nigeria,and compares findings with U.S NHANES data using WHO growth standards
## RESEARCH QUESTION
Is  BMI associated with systolic and diastolic blood pressure in school-aged(6-19 years) children from Uturu , Nigeria and  in U.S NHANES data ?
## DATA CLEANING AND PREPROCESSING 
NHANES dataset was cleaned and standardized before analysis to ensure fair comparison.
**1. Data Loading**
- **Uturu dataset**: Uturu_rawdata was loaded from CSV.
- **NHANES dataset**: Demographic ,Bp and BMI data for U.S children (2017-2018) was downloaded from CDC NHANES  public database for relevant cycle
- **WHO 2007 Growth Reference**: BMI-for-age reference tables were loaded.this included BMI percentiles and z-scores for boys and girls separately ,ages 5-19.
  
**2.  Column Selection and Standardization**:
  Only variable needed for the research question were kept: Age , Sex, BMI, SBP, DBP for NHANES data
  NHANES columns names were renamed to match Uturu dataset for consistency .Example: "RIDAGEYR " : "Age"

**3. Data Type Conversion**
  Sex in NHANES data was converted to a standard format so both datasets use the same labels for analysis
**4. Missing Data Handling**
rows with missing values in Age,BMI,SBP,DBP were removed
**5. Duplicates Data Handling**
rows that have duplicate ,the duplicate was removed .
**6. Age Filtering**
Only children aged 6-19years were kept to match the study scope 
**7. 
  
## METHODS
- **Study Population and Age Stratification**: Analysis was performed across aged groups 6-19 years for both uturu,Nigeria school children and U.S NHANES data. Age stratification was used to test if the BMI-BP relationship changes with age.
- **Significance**: Permutation-based Monte Carlo test with 10,000 iterations to generate empirical null distribution and p-values
- **Correlation**: Spearman rank correlation between BMI z-score and SBP/DBP
- **Visualization**:
  1. **Scatter plots**: BMI z-score 
