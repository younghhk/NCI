# Cancer Research Software Repository


A collection of tools for modeling cancer incidence, survival, biomarker selection, and risk prediction model development — designed to advance reproducible and data-driven cancer research.


### Repository Structure at a Glance

This repository is organized into four conceptual layers that reflect the full research pipeline:

- 🧱 **Data Foundations**  
  Real-world data sources, survey design, and population-level estimation

- 📐 **Core Statistical Methods**  
  Effect measures, survival analysis, causal inference, and evidence synthesis

- 🤖 **Advanced Machine Learning and High-Dimensional Methods**  
  Modern statistical learning, variable selection, and omics-scale modeling

- 🌍 **Domain Applications and Impact**  
  Applied cancer, behavioral, and population health research


## 📑 Contents

- [Data Foundations](#data-foundations)
  - [Population Health & Cancer Surveillance Research](#population-health--cancer-surveillance-research)
  - [Survey Data Methodology](#survey-data-methodology)
  - [Datasets & Codebooks](#datasets--codebooks)

- [Core Statistical Methods](#core-statistical-methods)
  - [Survival Analysis](#survival-analysis)
  - [Causal & Mediation Methods](#causal--mediation-methods)
  - [Meta-Analysis](#meta-analysis)
  - [Quantile Methods in Cancer Research](#quantile-methods-in-cancer-research)

- [Advanced Machine Learning and High-Dimensional Methods](#advanced-machine-learning-and-high-dimensional-methods)
  - [High-Dimensional Statistical Learning](#high-dimensional-statistical-learning)
  - [Biomarker and Metabolomics Research](#biomarker-and-metabolomics-research)

- [Domain Applications and Impact](#domain-applications-and-impact)
  - [Physical Activity & Sleep Epidemiology](#physical-activity--sleep-epidemiology)
  - [Health Disparities & Decomposition Methods](#health-disparities--decomposition-methods)
  - [Infectious Disease & Molecular Epidemiology](#infectious-disease--molecular-epidemiology)
  - [Radiation Epidemiology](#radiation-epidemiology)
  - [Clinical Trials Methods](#clinical-trials-methods)

---
# Data Foundations
🧱 Real-world data generation, survey design, and population-level estimation.

##  Population Health & Cancer Surveillance Research 

Tools for large-scale population health surveillance, cancer burden estimation, and standardized rate computation using registry and national data.

### [Healthy Eating Index (HEI) Software](https://github.com/younghhk/HEI)
R-based implementation of **HEI-2020** used widely in diet–cancer epidemiology to quantify diet quality in large cohorts such as NHANES.

### [Projecting Expected Cancer Cases](https://github.com/younghhk/expectedCases)


A tool for estimating expected cancer cases using age- and sex-specific incidence and mortality rates, providing an automated framework for cancer projections.

### [IBM-Calc](https://github.com/younghhk/SEER)

R functions for computing age-standardized Incidence-Based Mortality (IBM) rates and rate ratios, including methods to address small-count bias and variance estimation.



---
## Survey Data Methodology
📊 Design-based inference for complex survey data.

Methods and tools for analyzing complex survey data in population health and cancer epidemiology,  design-based inference, bias correction, and reproducibility.

All materials are maintained in a single repository with topic-specific subdirectories:
https://github.com/younghhk/survey-data-methodology

### [Complex Survey Design & Weighting](https://github.com/younghhk/survey-data-methodology/tree/main/design-weighting)
Design-based variance estimation, survey weights, strata, and PSU handling for nationally representative datasets such as NHANES.
<!--
### [Measurement Error & Validation Studies](https://github.com/younghhk/survey-data-methodology/tree/main/measurement-error)
Approaches to correcting self-reported exposure bias using biomarker calibration and validation substudies.

### [Small Area Estimation and Sparse Cells](https://github.com/younghhk/survey-data-methodology/tree/main/small-area-estimation)
Methods for stabilizing estimates in subpopulations with limited sample sizes, including shrinkage and pooling strategies.

-->

### [Missing Data in Survey Contexts](https://github.com/younghhk/survey-data-methodology/tree/main/MI)
Handling item nonresponse and unit nonresponse under simple random/ complex sampling designs.

---
##  Datasets & Codebooks

### [NHANES](https://github.com/younghhk/NHANES)

Documentation, variable descriptions, and examples for the National Health and Nutrition Examination Survey.

---

# Core Statistical Methods
📐 Principled modeling, interpretation, and inference for epidemiologic research.


### Effect Measures and Interpretation

### [Absolute Risk vs Relative Risk](https://github.com/younghhk/AR-RR)

An overview of absolute and relative risk, including:

* interpretation of each measure
* when each scale is most informative
* examples of additive versus multiplicative interaction



---

##  Survival Analysis: Concepts, Tools, and Applications

⏱️ Time-to-event modeling, prediction, and interpretation.

### [Delayed Entry in Cox Models](https://github.com/younghhk/Survival-Analysis#sec-time-scale-delayed-entry)
Guidance on handling left truncation and aligning participant risk intervals with the correct time scale.

### [Adjusted Survival Curves](https://github.com/younghhk/Survival-Analysis#sec-adjusted-survival)
Approaches to estimating survival curves adjusted for covariates in Cox models, including marginal and conditional methods.

### [Survival Prediction Using Machine Learning](https://github.com/younghhk/Survival-Analysis#survival-prediction-using-machine-learning)
Examples of using random survival forests, neural networks, and boosting methods for risk prediction.


### [Tutorial: Quantile Regression for Survival Data](https://academic.oup.com/pcm/article/2/2/90/5520072)
Introductory explanation of quantile-based approaches for censored survival outcomes.

### [Quantile Regression for Survival Data: FAQ for Epidemiologists](https://github.com/younghhk/CRQ)
A Q&A explaining identifiability issues when events are rare, why censored quantile regression may fail, and recommended alternatives for epidemiologic studies.

---

##  Causal & Mediation Methods

### [Planning Mediation Analysis](https://github.com/younghhk/Mediation-Analysis)

Framework for selecting appropriate mediation analysis strategies in observational cancer research.

### [High-Dimensional Mediation Analysis](https://github.com/younghhk/Moore)

Mediation methods tailored for high-dimensional omics data such as methylation and gene expression.

🔒 Access restricted to authorized collaborators.


---
##  Meta-Analysis and Evidence Synthesis

### [Meta-Analysis for Clinical Research](https://github.com/younghhk/Meta-Analysis)

Key concepts, formulas, and methods for fixed-effect and random-effects meta-analysis.

---
## Quantile Methods in Cancer Research

* Demographic associations with leukocyte telomere length (in revision)
* [CpG associations with short vs long cancer survival](https://academic.oup.com/pcm/article/2/2/90/5520072)
* Distributional analyses of racial/ethnic disparities in breast cancer survival

--- 

# Advanced Machine Learning and High-Dimensional Methods
🤖 Scalable learning methods for high-dimensional and complex biomedical data.


## High-Dimensional Statistical Learning

### [Variable Selection & Stability](https://github.com/younghhk/VS)
Tools for high-dimensional biomarker selection using **LASSO**, **Elastic Net**, **Group LASSO**, and **Stability Selection**, supporting reproducible variable selection and score development.


###  Recent Methodological Work

- [Genetic Effects in Longitudinal Phenotypes (2025)](https://pubmed.ncbi.nlm.nih.gov/40893136/)
- [Quantile Forward Regression for High-Dimensional Survival (2023)](https://doi.org/10.1007/s10985-023-09603-w)
- [Varying-Coefficient Regional Quantile via KNN–LASSO (2023)](https://doi.org/10.1002/sim.9839)
- [Inference for High-Dimensional Censored Quantile Regression (2023)](https://pubmed.ncbi.nlm.nih.gov/37309513/)



###  Earlier Developments  
*(Foundational contributions that shaped later work)*

- [Sequentially Conditional GLMs (2020)](https://pubmed.ncbi.nlm.nih.gov/31350909/)
- [Multiclass LDA with Ultrahigh-Dimensional Features (2019)](https://pubmed.ncbi.nlm.nih.gov/31009070/)
- [Forward Regression for Cox Models (2019)](https://pubmed.ncbi.nlm.nih.gov/31007300/)
- [Lq-Norm Learning (2018)](https://pubmed.ncbi.nlm.nih.gov/32742137/)
- [IPOD: Screening Ultrahigh-Dimensional Covariates with Survival Outcomes (2018)](https://doi.org/10.1111/biom.12820)
- [Conditional Screening with Survival Data (2018)](https://doi.org/10.1007/s10985-016-9387-7)
- [Partition-Based Screening (2017)](https://doi.org/10.1093/biomet/asx052)
- [Quantile-Adaptive Model-Free Screening (2013)](https://github.com/younghhk/QA)


---
## Biomarker and Metabolomics Research

### [IDATA Metabolomics Project](https://github.com/younghhk/IDATA)
Metabolomics analyses from the **IDATA** biomarker validation study evaluating diet and activity reporting for use in cancer epidemiology.  

🔒 Access restricted to authorized collaborators.

### [Liver Cancer Metabolomics Study](https://github.com/younghhk/livercancer)
Identifying metabolites associated with hepatocellular carcinoma (HCC) and intrahepatic cholangiocarcinoma (ICC).

🔒 Access restricted to authorized collaborators.

---
# Domain Applications and Impact

🌍 Applied research translating methods into population and clinical insights.


## Transplantation and Hematologic Malignancies

### [GS-BMT Study: Population and Methods](https://github.com/younghhk/HCT)

🔒 Access restricted to authorized collaborators.

## Physical Activity & Sleep Epidemiology

### [Attributes Associated with Physical Activity Outcomes Using Machine Learning](https://github.com/younghhk/Kebede)

Machine learning applied to demographic, socioeconomic, health, and other individual attributes to characterize associations with two physical activity outcomes analyzed separately.

🔒 Access restricted to authorized collaborators.

### [ICC for Sleep Measurements](https://github.com/younghhk/Sleep)

Tutorial on computing ICCs in multilevel sleep data with day-, window-, and person-level variance components.

🔒 Access restricted to authorized collaborators.

### [LMM/GLMM vs GEE](https://github.com/younghhk/MM)

Comparison of mixed-effects models vs GEE for clustered and longitudinal epidemiologic data.

---

##  Health Disparities & Decomposition Methods

### [Peters–Belson Decomposition](https://github.com/younghhk/Disparity-Decomposition#petersbelson-decomposition-on-the-proportion-of-death-black-vs-white)

Quantifying survival disparities explained by measurable vs residual factors.

### [Quantile-Based Decomposition](https://pmc.ncbi.nlm.nih.gov/articles/PMC12456447/)

Distributional disparity analyses for complex survey data.

### [Longitudinal Disparity Decomposition](https://doi.org/10.10093/biostatistics/kxaf044)

Evaluating disparities that evolve over follow-up.

---
## Infectious Disease & Molecular Epidemiology

### [Malaria Complexity Project](https://github.com/younghhk/Malaria)
Complexity of Infection (COI) analyses examining malaria transmission intensity, parasite exposure, and Burkitt lymphoma risk.

🔒 Access restricted to authorized collaborators.

---

##  Radiation Epidemiology

### [Radiation Epidemiology Risk Modeling in R](https://github.com/younghhk/Radiation-epi)

Overview of **Colossus** and **Epicure** for dose–response modeling, survival analysis, and radiation risk estimation.


---


##  Clinical Trials Methods

### [Training Resources](https://github.com/younghhk/ClinicalTrials)

Materials on clinical trial design, power, sample size, and key methodological principles.



---
## Author

**Hyokyoung “Grace” Hong**  
Senior Investigator, Biostatistics Branch (BB), Division of Cancer Epidemiology and Genetics (DCEG), NIH  

Email: [grace.hong@nih.gov](mailto:grace.hong@nih.gov)  
DCEG profile: https://dceg.cancer.gov/about/staff-directory/hong-grace  
GitHub: https://github.com/younghhk





