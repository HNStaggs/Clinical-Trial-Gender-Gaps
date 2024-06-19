# Identifying Gender Gaps in Clinical Trial Research

## Project Background
There is a historical gender gap in clinical trial participation. The National Institutes of Health (NIH) Revitalization Act of 1993 introduced the requirement for females, in addition to underrepresented racial and ethnic minority populations, to be included in clinical trial research.
The goal of this project is to classify the sex of participants in clinical trials from text descriptions of research goals pulled from the ClinicalTrials.gov API. More info about the API can be found here: https://clinicaltrials.gov/data-api/api. 

## Methods
Text descriptions of clinical research trials were refined through a series of text processing steps.  Using natural lanaguage processing, classification models were trained and tested to examine disparities in research topics between studies focusing on females and those focusing on males. 

## Model Implications
Researchers can use the coefficients of these models to investigate gender representation in various fields and areas of study, aiding grant applications and literature reviews. Grant funding agencies can use the output of these models to invest money in areas of research with gender gaps.

## Programming Language
* Python - Jupyter Notebook

## Notes on Model Use
* Adjust max_requests parameter in the API call depending on how much data you'd like to retrieve
* Data from API call is saved as .csv and .json to the "data_files" folder to prevent subsequent duplicate calls to the API
* The models will output the research topics with gender gaps into the folder "gender_gaps" as a .csv file
* Male coded as 1, female as 0
* SVM Coefficient Interpretation: Positive Values indicate "Male", and negative values indicate "Female"
* Logistic Regression Coefficient Interpretation: Odds ratios above 1 increase odds for "male", odd ratios below 1 decrease odds for "male" i.e., increase for "female"
* Naive Bayes Coefficient Interpreation: The order of the ratio show which sex that token is overrepresented for. For examle, 0:1 with a value of 15 would indiciated 15x more studies done on that topic for females compared to males, and 1:0 with a value of 5 would indicate 5x more studies done on that topic for males compared to females. 

## References
ClinicalTrials.gov API. Clinicaltrials.gov. (n.d.). 

  
