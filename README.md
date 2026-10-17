# SDGs and Crowdfunding Dataset

## 1. Overview

This repository contains the research data and supporting materials for the study *The Impact of Sustainable Development Goals on the Success of Online Crowdfunding Campaigns: An Analysis Through Natural Language Processing Techniques*.

The study examines the relationship between the Sustainable Development Goals (SDGs) and the success of online crowdfunding campaigns using campaign-level data, natural language processing (NLP), and econometric analysis. The dataset covers Kickstarter campaigns from 2020 to 2024.

## 2. Data Source

The original data were downloaded from [Web Robots – Kickstarter Datasets](https://webrobots.io/kickstarter-datasets/), a provider of datasets collected from Kickstarter projects.

For this research, campaign data covering five years, from 2020 through 2024, were collected and processed to construct a consolidated dataset suitable for empirical analysis.

## 3. Data Collection, Merging, and Cleaning

The downloaded data were initially organized into monthly folders, with each folder containing numerous individual Excel files. Depending on the month, approximately 50–200 files were available.

The data preparation process involved the following steps:

1. **Monthly consolidation:** Individual files within each monthly folder were merged into a single monthly dataset.
2. **Yearly consolidation:** The 12 monthly datasets for each year were combined to produce one dataset for each year.
3. **Duplicate removal:** Duplicate campaign records were identified and removed during the data cleaning process.
4. **Five-year consolidation:** The five annual datasets, covering 2020–2024, were combined into one consolidated dataset.

The resulting datasets provided the foundation for text preprocessing, SDG classification, variable construction, and econometric analysis.

## 4. Campaign Description Preprocessing

After consolidating the campaign data, campaign descriptions were extracted for NLP-based analysis. The text was cleaned and prepared before being processed by the SDG classification packages.

The preprocessing workflow included:

- **Text cleaning:** Removing unwanted text elements and punctuation.
- **Stop-word removal:** Removing common words with limited analytical value where appropriate.
- **Tokenization:** Separating campaign descriptions into individual words or tokens.
- **Lemmatization:** Converting words into their base or dictionary forms.

These steps were intended to standardize the campaign descriptions and prepare them for subsequent text classification.

## 5. NLP-Based SDG Classification

Two NLP-based tools, **SDGdetector** and **Text2SDG**, were used to identify campaign descriptions related to the Sustainable Development Goals.

The outputs from SDGdetector were used to construct the SDG-related explanatory variables for the main regression analysis. Text2SDG generated an alternative set of SDG classifications for robustness checks.

The classification outputs were retained separately and subsequently integrated with the consolidated campaign data.

## 6. Construction of the Final Analysis Datasets

Following the NLP classification process, the classification results were combined with the campaign data containing the dependent variables and control variables required for the econometric analysis.

The dependent variables represented crowdfunding success, including the amount pledged and the number of backers. The explanatory variables captured the relationship between campaign content and the SDGs, including an overall SDG-related indicator and individual SDG variables. Relevant campaign characteristics and other controls were also incorporated into the analysis datasets.

Two final datasets were prepared:

### 6.1 Main Regression Dataset

This dataset combines campaign outcomes, control variables, and SDG classifications obtained using SDGdetector. It was prepared for the primary econometric analysis.

### 6.2 Robustness-Check Dataset

This dataset combines the corresponding campaign outcomes and control variables with the alternative SDG classifications obtained using Text2SDG. It was prepared to assess whether the main findings remain consistent when an alternative NLP-based classification approach is used.

Maintaining these datasets separately allows the main analysis and robustness checks to be distinguished clearly.

## 7. Econometric Analysis

The final datasets were used to examine the relationship between SDG-related campaign content and crowdfunding success.

The main regression analysis considered two outcome variables:

- The logarithm of the amount pledged.
- The logarithm of the number of backers.

The models incorporated relevant campaign-level controls and year fixed effects, alongside other specified categorical controls. These specifications were designed to examine the association between SDG-related campaign content and funding outcomes while accounting for observed differences across campaigns and years.

The robustness analysis used the alternative SDG classifications generated by Text2SDG to evaluate the consistency of the main findings across classification methods.

## 8. Repository Organization

The repository is organized into five main folders:

- **Final Data Used for Regression Models:** Contains the final datasets prepared for the main regression analysis and robustness checks.
- **Overall & Data yearly after merging_cleaning:** Contains the consolidated annual datasets and other merged and cleaned campaign data.
- **R packages NLP Results:** Contains the outputs generated by the SDG classification packages, including SDGdetector and Text2SDG.
- **Sentiment Analysis of the campaign description:** Contains data and outputs associated with sentiment analysis of campaign descriptions.
- **codes and variables decodes:** Contains supporting code, variable definitions, and documentation.

Together, these materials document the main stages of the research workflow, from data consolidation and text processing to NLP classification and the preparation of the final econometric datasets.

## 9. Reproducibility and Data Use

The repository is intended to support research transparency, documentation, and further academic work on SDGs, crowdfunding, and NLP-based empirical methods.

Researchers seeking to reproduce or extend the analysis should consult the included code and variable documentation. The original data were obtained from Web Robots; users should review the provider's terms and applicable licensing conditions before redistributing the original data or derived datasets.

**Original data source:** [https://webrobots.io/kickstarter-datasets/](https://webrobots.io/kickstarter-datasets/)

## 10. Citation

If these materials are used in academic work, please cite the associated research study when its formal publication details become available.
