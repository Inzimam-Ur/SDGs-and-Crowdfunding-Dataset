# SDGs and Crowdfunding Dataset

## 1. Overview

This repository contains data and supporting materials for the study *The Impact of Sustainable Development Goals on the Success of Online Crowdfunding Campaigns: An Analysis Through Natural Language Processing Techniques*. It uses Kickstarter campaign data from 2020–2024.

**Data source:** [Web Robots – Kickstarter Datasets](https://webrobots.io/kickstarter-datasets/)

## 2. Data Collection and Cleaning

Monthly campaign files were merged into yearly and consolidated datasets, with duplicate records removed.

**Folder:** [Overall and Yearly Data After Merging and Cleaning](https://github.com/Inzimam-Ur/SDGs-and-Crowdfunding-Dataset/tree/main/Overall%20and%20Yearly%20Data%20After%20Merging%20and%20Cleaning)

## 3. Campaign Text Preprocessing

Campaign descriptions were cleaned and prepared for text analysis using standard preprocessing steps, including tokenization and lemmatization.

## 4. NLP-Based SDG Classification

SDGdetector was used for the main SDG classification, while Text2SDG provided alternative classifications for robustness checks.

**Folder:** [R Packages NLP Results](https://github.com/Inzimam-Ur/SDGs-and-Crowdfunding-Dataset/tree/main/R%20packages%20NLP%20Results)

## 5. Final Analysis Datasets

The campaign data, SDG classifications, outcome variables, and controls were combined to prepare datasets for the main analysis and robustness checks.

**Folder:** [Final Data Used for Regression Models](https://github.com/Inzimam-Ur/SDGs-and-Crowdfunding-Dataset/tree/main/Final%20Data%20Used%20for%20Regression%20Models)

## 6. Econometric Analysis

Regression models examine the relationship between SDG-related campaign content and crowdfunding success, measured by the amount pledged and number of backers.

## 7. Regression Results

The PDF contains regression tables for the main analysis and robustness checks.

**Folder:** [Regression Results](https://github.com/Inzimam-Ur/SDGs-and-Crowdfunding-Dataset/tree/main/Regression%20Results) | [View Regression Results (PDF)](Regression%20Results/Regression%20Results.pdf)

## 8. Code and Documentation

Supporting documents provide code-related information, variable definitions, and country reference materials.

**Folder:** [Codes and Variable Definitions](https://github.com/Inzimam-Ur/SDGs-and-Crowdfunding-Dataset/tree/main/codes%20and%20variables%20decodes)

## 9. Data Use and Citation

Users should review the original data provider's terms before redistributing datasets. Please cite the associated study when its publication details become available.
