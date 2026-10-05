# FSW Research Data Analysis & Machine Learning

## Overview

This project presents a comprehensive data analysis and machine learning
study of **Friction Stir Welding (FSW)** research data collected from
the literature.

The dataset contains approximately **1,680 experimental records**
covering FSW studies published between **2003 and 2026**, with
information on materials, joint types, tool geometry, process
parameters, and mechanical properties.

The analysis combines exploratory data analysis, statistical analysis,
machine learning, clustering, feature importance, and parameter-level
insights to understand relationships between FSW process conditions and
material performance.

## Objectives

-   Clean and preprocess the FSW research dataset.
-   Explore publication, material, joint-type, and process-parameter
    trends.
-   Analyse relationships between process parameters and mechanical
    properties.
-   Identify factors associated with Ultimate Tensile Strength (UTS) and
    hardness.
-   Develop machine-learning models for UTS and hardness prediction.
-   Classify joint types using process parameters.
-   Identify material/process groupings using clustering.
-   Examine parameter combinations associated with higher UTS.
-   Highlight potential research gaps in the literature.

## Analysis Performed

### 1. Data Cleaning & Preprocessing

-   Standardized column names.
-   Converted numerical variables to appropriate formats.
-   Examined missing values.
-   Created derived features such as:
    -   Heat Index = Rotation RPM / Traverse Speed
    -   Shoulder-to-Probe Ratio

### 2. Exploratory Data Analysis

Analysed: - Publication trends from 2003--2026 - Frequently studied
materials - Joint-type distribution - Tool-material usage - Process
parameter distributions - Mechanical-property distributions - UTS and
hardness across joint types and materials

### 3. Statistical Analysis

Performed: - Correlation analysis - Pearson correlation analysis -
One-way ANOVA - Comparison of UTS across rotation-speed categories -
Analysis of process parameters and mechanical properties

### 4. Machine Learning --- UTS Prediction

Compared: - Linear Regression - Ridge Regression - Random Forest
Regressor - XGBoost Regressor

Models were evaluated using: - R² - RMSE - MAE - 5-fold cross-validation
for selected models

### 5. Hardness Prediction

An XGBoost regression model was developed to predict **Vickers Hardness
(HV)** from process parameters, tool geometry, and material/joint
information.

### 6. Feature Importance & SHAP

Used: - Random Forest feature importance - SHAP feature importance -
SHAP beeswarm analysis

to investigate which variables contribute most strongly to UTS
predictions.

### 7. Clustering

Applied: - StandardScaler - K-Means clustering - PCA dimensionality
reduction - Elbow-method analysis

to identify groups of similar FSW process conditions.

### 8. Joint-Type Classification

A Random Forest classifier was developed to distinguish between the two
dominant joint types: - Butt - Lap

### 9. Parameter Optimization Insights

Investigated: - RPM × traverse-speed interactions - Shoulder diameter
vs. UTS - Highest-performing experimental parameter combinations

### 10. Research Gaps

Analysed material frequency and property coverage over time to identify
areas that appear less explored in the collected literature.

## Key Dataset Highlights

-   **\~1,680 experimental records**
-   **44 features**
-   Literature coverage: **2003--2026**
-   Process parameters include rotation speed, traverse speed, tool
    geometry, plunge depth, axial load and torque.
-   Mechanical properties include UTS, hardness, strain and weld
    efficiency.

## Technologies & Libraries

**Programming:** Python

**Libraries:** - Pandas - NumPy - Matplotlib - Seaborn - SciPy -
Statsmodels - Scikit-learn - XGBoost - SHAP

**Methods:** - Exploratory Data Analysis - Statistical Testing -
Regression - Classification - Random Forest - XGBoost - PCA - K-Means
Clustering - Feature Importance - SHAP Analysis

## Repository Structure

``` text
FSW-Research-Data-Analysis/
│
├── FSW_Analysis_executed.ipynb
└── README.md
```

## Note

This repository contains the analysis notebook developed for the FSW
research dataset. The results and interpretations are based on the
records available in the analysed dataset and are intended for research
and analytical exploration.

## Author

**Pawar Sai Kiran**\
B.Tech. Materials Science and Engineering\
Indian Institute of Technology Gandhinagar
