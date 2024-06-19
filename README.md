# Identifying Gender Gaps in Clinical Trial Research

## Project Background
There is a historical gender gap in clinical trial participation. The NIH Revitalization Act of 1993 introduced the requirement for females to be in clinical trial research.
The goal of this project is to classify the sex of participants in clinical trials from text descriptions of research goals pulled from the ClinicalTrials.gov API. 

## Methods
Using natural lanaguage processing, classification models were trained and tested to examine disparities in research topics between studies focusing on females and those focusing on males. 

## Model Implications
Researchers can use the coeffcieints of these models to investigate gender representation in various fields and areas of study, aiding grant applications and literature reviews. Grant funding agencies can use the output of these models to invest money in areas of research with gender gaps.

## Programming Language
* Python - Jupyter Notebook

## Notes on Model Use
* Adjust max_requests parameter in the API call depending on how much data you'd like to retrieve
* Data from API call is saved as .csv and .json to the data_files folder to prevent subsequent duplicate calls to the API
  
