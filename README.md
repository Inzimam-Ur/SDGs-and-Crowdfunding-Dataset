SDGs and Crowdfunding Dataset

Overview

This repository contains the data and supporting materials for the study The Impact of Sustainable Development Goals on the Success of Online Crowdfunding Campaigns: An Analysis Through Natural Language Processing Techniques.

The study examines the relationship between SDG-related campaign content and crowdfunding success using Kickstarter data from 2020–2024, natural language processing (NLP), and econometric analysis.

Original data source: Web Robots – Kickstarter Datasets

Research Workflow

The research involved consolidating monthly campaign files into yearly and combined datasets, cleaning duplicate records, preprocessing campaign descriptions, and identifying SDG-related content using SDGdetector and Text2SDG. The resulting datasets were used for the main regression analysis and robustness checks.

Repository Contents

Overall and Yearly Data After Merging and Cleaning — Consolidated yearly and combined datasets.

R Packages NLP Results — SDGdetector and Text2SDG outputs and supporting materials.

Final Data Used for Regression Models — Main analysis and robustness-check datasets.

Regression Results — View regression tables (PDF).

Codes and Variable Definitions — Supporting code and documentation.

Analysis

The regression models examine two measures of crowdfunding success: the amount pledged and the number of backers. The main analysis uses SDGdetector classifications, while Text2SDG classifications are used for robustness checks. The models include relevant campaign-level controls and year fixed effects.
