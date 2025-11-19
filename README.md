# 🧬 Cancer Research Software Repository
A collection of tools for modeling cancer incidence, survival, biomarker selection, and risk prediction model development — designed to advance reproducible and data-driven cancer research.

## Contents


### 🥗 [Software for Computing Healthy Eating Index (HEI)](https://github.com/younghhk/HEI)

An R-based implementation of the **Healthy Eating Index (HEI-2020)** scoring system using **NHANES** and **FPED** data.

This tool reproduces the official **USDA/NCI methodology** for computing total and component HEI-2020 scores, allowing researchers to evaluate dietary quality directly within `R`.

---

### 🪢 Mediation Analysis in Genetic Association Studies

- [**Planning Mediation Analysis**](https://github.com/younghhk/Mediation-Analysis)  
  A workflow for planning mediation analysis in observational cancer research.  
  This resource helps researchers determine the appropriate analytical framework based on study design, including outcome type, mediator dimensionality, and confounder structure.

- [**High-Dimensional Mediation Analysis**](https://github.com/younghhk/Moore)  
  A framework for mediation analysis in high-dimensional settings such as methylation, gene expression, and other omics data.

🔒 Access to this repository is currently limited to authorized collaborators.

---

### 📘 Mixed-Effects Modeling

- 📏 [**ICC for Sleep Measurements**](https://github.com/younghhk/Sleep)  
  A guide to computing intraclass correlation coefficients (ICCs) in multilevel sleep data with day, season, and person effects.

  This tutorial explains:
  - how to specify the appropriate mixed-effects model  
  - how to interpret ICC as a measure of reliability  
  - how to compute ICC from model-based variance components  

🔒 Access to this repository is currently limited to authorized collaborators.

---  
### 📈 [Projecting Expected Cancer Cases](https://github.com/younghhk/expectedCases)

A tool for estimating expected cancer cases using age- and sex-specific incidence and mortality rates, providing an automated framework for cohort-based cancer projections.

  🔒 Access to this repository is currently limited to authorized collaborators until the program is fully verified.

---
### 🧮 [IBM-Calc: A Computational Tool for Estimating Age-Standardized Incidence-Based Mortality and Rate Ratio Confidence Intervals](https://github.com/younghhk/SEER)

  This repository provides R functions to compute age-adjusted Incidence-Based Mortality (IBM) rates and rate ratios.
The methods include adjustments for small-count bias and variance estimation, making them suitable for rare cancers and small populations.

  🔒 Access to this repository is currently limited to authorized collaborators until the program is fully verified.

---

### 📊 [Meta-Analysis for Clinical Research](https://github.com/younghhk/Meta-Analysis)

   This repository provides an overview, key concepts, and essential formulas for performing meta-analysis in clinical research, including fixed-effect and random-effects models.

---  
###  Survival Analysis



- [Handling Delayed Entry in Cox Models](https://github.com/younghhk/Survival-Analysis#sec-time-scale-delayed-entry)  
  Explores methods to correctly handle **left truncation** and align entry times in Cox proportional hazards models.

- [Adjusted Survival Curve Estimation from the Cox Proportional Hazards Model](https://github.com/younghhk/Survival-Analysis#sec-adjusted-survival)  
  Demonstrates how to estimate **adjusted survival curves** that account for covariate distributions or population-level effects.

- [Survival Prediction Using Machine Learning](https://github.com/younghhk/Survival-Analysis#survival-prediction-using-machine-learning)  
  Covers the use of **machine learning algorithms** (e.g., random survival forests, deep learning, and gradient boosting) for survival prediction and risk stratification.

---
###  Disparity Decomposition Methods


- [Peters–Belson Decomposition of the Proportion of Death](https://github.com/younghhk/Disparity-Decomposition#petersbelson-decomposition-on-the-proportion-of-death-black-vs-white)  
  Applies the **Peters–Belson framework** to estimate the proportion of survival disparities between groups (e.g., Black vs. White populations) explained by measurable risk factors versus residual differences.

- [Quantile-Based Disparity Decomposition for Complex Survey Data (Upper-Tail BMI / Lower-Tail Telomere)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12456447/)  
  Applies **quantile-based decomposition methods** to complex survey data, analyzing disparities across specific portions of the distribution (e.g., upper-tail BMI or lower-tail telomere length) to uncover subgroup-specific effects often obscured by mean-based approaches.

- [Decomposition of Longitudinal Disparities](https://doi.org/10.10093/biostatistics/kxaf044) *(in press, available soon)*  
  Extends decomposition techniques to evaluate how disparities **evolve dynamically over follow-up time**.



---
### Quantile Regression for Cancer Research: Beyond the Mean



- Investigates whether **sex is associated differently across the telomere-length distribution**

- Identifies **CpG sites linked to elevated LINE-1 activity** (via total transposable element counts) 

- Examines whether **race/ethnicity influences short-term versus long-term breast cancer survival differently**, capturing distributional heterogeneity often missed by mean-based models.

---
### 🧠 High-Dimensional Statistical and Machine Learning Methods

### Recent Works

- [Mixed Modeling Approach for Genetic Effects in Longitudinal Phenotypes (2025)](https://pubmed.ncbi.nlm.nih.gov/40893136/)

- [Quantile Forward Regression for High-Dimensional Survival Data (2023)](https://doi.org/10.1007/s10985-023-09603-w)

- [Varying-Coefficient Regional Quantile via KNN–LASSO (2023)](https://doi.org/10.1002/sim.9839)

- Discovery of Gene-Specific Time Effects on Survival (2024) — *Book Chapter*

- [Inference for High-Dimensional Censored Quantile Regression (2023)](https://pubmed.ncbi.nlm.nih.gov/37309513/)



### Earlier Developments

- Sequentially Conditional GLMs (2020)

- Multiclass LDA with Ultrahigh-Dimensional Features (2019)

- Forward Regression for Cox Models (2019)

- Lq-Norm Learning (2018)

- [IPOD Screening (2018)](https://doi.org/10.1111/biom.12820)

- [Conditional Screening with Survival Data (2018)](https://doi.org/10.1007/s10985-016-9387-7)

- [Partition-Based Screening (2017)](https://doi.org/10.1093/biomet/asx052)

- [Quantile-Adaptive Model-Free Screening (2013)](https://doi.org/10.1214/13-AOS1087)

 ---


### 🧑‍💻 Author

**Hyokyoung "Grace" Hong**  
📧 [grace.hong@nih.gov](mailto:grace.hong@nih.gov)  

Senior Investigator<br>
Biostatistics Branch<br>
Division of Cancer Epidemiology and Genetics<br>
National Cancer Institute<br>
National Institutes of Health

💬 For questions, feedback, or collaboration inquiries, please feel free to reach out via email.




