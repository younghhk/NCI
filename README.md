# Cancer Research Software Repository

## Contents
- [1. SEER Cancer Data Analysis 🔒 (Collaborators Only)](#1-seer-cancer-data-analysis)

- [2. Survival Analysis](https://github.com/younghhk/Survival-Analysis)
  - [2.1 Choosing the Time Scale and Handling Delayed Entry in Cox Models](https://github.com/younghhk/Survival-Analysis#sec-time-scale-delayed-entry)
  - [2.2 Adjusted Survival Curve Estimation from the Cox Proportional Hazards Model](https://github.com/younghhk/Survival-Analysis#sec-adjusted-survival)
  - [2.3 Survival Prediction Using Machine Learning 🔒 (Collaborators Only)](https://github.com/younghhk/Survival-Analysis#survival-prediction-using-machine-learning)

- [3. Cancer Disparity Decomposition Methods](https://github.com/younghhk/Disparity-Decomposition)
  - [3.1 Peters–Belson Decomposition of the Proportion of Death](https://github.com/younghhk/Disparity-Decomposition#petersbelson-decomposition-on-the-proportion-of-death-black-vs-white)
  - [3.2 Quantile-Based Decomposition (Lower-Tail BMI / Telomere)](https://github.com/younghhk/Disparity-Decomposition#quantile-based-disparity-decomposition-focus-on-lower-bmi)
  - [3.3 Time-Dependent Disparity Decomposition](https://github.com/younghhk/Disparity-Decomposition#3-time-dependent-disparity-decomposition--narrative-no-formulas)

- [4. Quantile Regression for Cancer Research: Beyond the Mean](https://github.com/younghhk/Quantile-Regression)
  - 4.1 Is sex associated differently at **lower** vs **higher** telomere-length quantiles, or is the effect constant across quantiles?
  - 4.2 Identifying CpG sites associated with **high LINE-1 activity** (via **total TE counts**) using upper-quantile modeling
  - 4.3 Do race/ethnicity effects differ for **short** vs **long** breast cancer survival? *(use censored quantile methods)*

- [5. High-Dimensional Feature (Biomarker) Selection](https://github.com/younghhk/Feature-selection)
  - [5.1 Mixed Modeling Approach for Genetic Effects in Longitudinal Phenotypes (2025)](https://github.com/younghhk/Feature-selection#mixed-2025)
  - [5.2 Discovery of Gene-Specific Time Effects on Survival (2024)](https://github.com/younghhk/Feature-selection#gene-time-2024)
  - [5.3 Inference for High-Dimensional Censored Quantile Regression (2023)](https://github.com/younghhk/Feature-selection#hd-cqr-2023)
  - [5.4 Quantile Forward Regression for High-Dimensional Survival Data (2023)](https://github.com/younghhk/Feature-selection#qfr-2023)
  - [5.5 Varying-Coefficient Regional Quantile via KNN–LASSO (2023)](https://github.com/younghhk/Feature-selection#vc-knn-lasso-2023)
  - [5.6 Sequentially Conditional GLMs (2020)](https://github.com/younghhk/Feature-selection#sc-glm-2020)
  - [5.7 Multiclass LDA with Ultrahigh-Dimensional Features (2019)](https://github.com/younghhk/Feature-selection#lda-2019)
  - [5.8 Forward Regression for Cox Models (2019)](https://github.com/younghhk/Feature-selection#cox-forward-2019)
  - [5.9 Lq-Norm Learning (2018)](https://github.com/younghhk/Feature-selection#lq-2018)
  - [5.10 IPOD Screening (2018)](https://github.com/younghhk/Feature-selection#ipod-2018)
  - [5.11 Conditional Screening (2018)](https://github.com/younghhk/Feature-selection#cs-2018)
  - [5.12 Partition-Based Screening (2017)](https://github.com/younghhk/Feature-selection#partition-2017)
  - [5.13 Quantile-Adaptive Model-Free Screening (2013)](https://github.com/younghhk/Feature-selection#qa-2013)
---


## 1. SEER Cancer Data Analysis

This repository provides example code and documentation for **SEER Cancer Registry data analysis**, focusing on **incidence-based mortality (IBM) rates**, **rate ratios**, and related survival analysis methods.





###  Features
- Functions to compute **incidence-based mortality rates** with small-count adjustments:
  - **Fay–Feuer method** (recommended for rare events)  
  - **Tiwari’s modification** (alternative adjustment)  
- Functions to estimate **rate ratios** with variance estimates using the **delta method**  
- Example workflows demonstrating SEER-based analyses  



### Example Workflow

```r
```r
# Load functions
source("IBM.R")

# Install package if needed
install.packages("readxl")

# Load the library
library(readxl)

# Read the Excel file
df <- read_excel("age_adjusted_data_grace.xlsx")


# Define index sets for comparison:
# Example: ER-negative, Non-Hispanic White vs Non-Hispanic Black, age 30–54
idx1 <- which(df$ER == "Negative" &
                df$Race == "Non-Hispanic White" &
                df$age_group_strata == "30 - 54")

idx2 <- which(df$ER == "Negative" &
                df$Race == "Non-Hispanic Black" &
                df$age_group_strata == "30 - 54")

# Compute DSRs and rate ratio with Fay–Feuer CI
compute_dsr_and_rr_for_subset(df, idx1, idx2,
                              "ER- & NHW & 30-54",
                              "ER- & NHB & 30-54",
                              "Subset",
                              ci_method = "fayfeuer")
```


###  Example 

An example SEER analysis is included:  
 [SEER_example.pdf](SEER_example.pdf)  



###  Resources
- [SEER Program Overview](https://seer.cancer.gov/)  
- [NCI Division of Cancer Epidemiology and Genetics](https://dceg.cancer.gov/)  



---
## 🔒 Repository Access

Some content is restricted to collaborators. To request access, please contact:

**Grace Hong**  
📧 [grace.hong@nih.gov](mailto:grace.hong@nih.gov)

*Tip: Include your GitHub username and affiliation in your request.*


