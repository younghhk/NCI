#  Research Software Repository

## Table of Contents
1. [SEER Cancer Data Analysis](#1-seer-cancer-data-analysis)
2. [Survival Prediction Using Machine Learning](#2-Survival-Prediction-Using-Machine-Learning)
3. [Other Topics](#3-other-topics)

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
## 2. [Survival Prediction Using Machine Learning](#2-survival-prediction-using-machine-learning)



###  Examples with allogeneic hematopoietic cell transplantation (HCT):

- **Model Performance (AUC Comparison):** [AUC.pdf](model_auc_comparison.pdf)  
- **Survival Curves (Kaplan–Meier):** [KM.pdf](km_plots.pdf)  
- **Risk Stratification (Random Survival Forests):** [Risk Stratification.pdf](rsf_risk_groups.pdf)  

###  Resources
- [Random Survival Forests Overview](https://www.randomforestsrc.org/articles/survival.html)  


---
## 🔒 Repository Access

The SEER repository is **private**.  
Access requests may be directed to:

**Grace Hong**  
📧 [grace.hong@nih.gov](mailto:grace.hong@nih.gov)  

