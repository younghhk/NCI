# Cancer Research Software Repository


A collection of tools for modeling cancer incidence, survival, biomarker selection, and risk prediction model development — designed to advance reproducible and data-driven cancer research.


## 📑 Contents

- [Core Epidemiologic Concepts](#core-epidemiologic-concepts)
- [Population Health & Cancer Surveillance Research](#population-health--cancer-surveillance-research)
- [Physical Activity & Sleep Epidemiology](#physical-activity--sleep-epidemiology)
- [Nutritional Epidemiology & Diet Quality](#nutritional-epidemiology--diet-quality)
- [Causal & Mediation Methods](#causal--mediation-methods)
- [Meta-Analysis & Evidence Synthesis](#meta-analysis--evidence-synthesis)
- [Survival Analysis & Methods Development](#survival-analysis--methods-development)
- [Health Disparities & Decomposition Methods](#health-disparities--decomposition-methods)
- [Quantile Methods in Cancer Epidemiology](#quantile-methods-in-cancer-epidemiology)
- [High-Dimensional Statistical Learning](#high-dimensional-statistical-learning)
- [Radiation Epidemiology](#radiation-epidemiology)
- [Clinical Trials Methods](#clinical-trials-methods)
- [Datasets & Codebooks](#datasets--codebooks)

---
##  Core Epidemiologic Concepts 📚

*(Foundational topics used across all domains)*

### [Absolute Risk vs Relative Risk](https://github.com/younghhk/AR-RR)

An overview of absolute and relative risk, including:

* interpretation of each measure
* when each scale is most informative
* examples of additive versus multiplicative interaction

### [Handling Missing Data](https://github.com/younghhk/MI)

Guidance on identifying **MCAR**, **MAR**, and **MNAR** mechanisms, with recommended strategies tailored to each type of missingness.

---
##  Population Health & Cancer Surveillance Research 🧬 

### [Projecting Expected Cancer Cases](https://github.com/younghhk/expectedCases)

A tool for estimating expected cancer cases using age- and sex-specific incidence and mortality rates, providing an automated framework for cancer projections.

### [IBM-Calc](https://github.com/younghhk/SEER)

R functions for computing age-standardized Incidence-Based Mortality (IBM) rates and rate ratios, including methods to address small-count bias and variance estimation.

🔒 Access currently limited to authorized collaborators.


---
## Physical Activity & Sleep Epidemiology 🏃‍♂️

### [Attributes Associated with Physical Activity Outcomes Using Machine Learning](https://github.com/younghhk/Kebede)

Machine learning applied to demographic, socioeconomic, health, and other individual attributes to characterize associations with two physical activity outcomes analyzed separately.

🔒 Access restricted to authorized collaborators.

### [ICC for Sleep Measurements](https://github.com/younghhk/Sleep)

Tutorial on computing ICCs in multilevel sleep data with day-, window-, and person-level variance components.

🔒 Access restricted to authorized collaborators.

### [LMM/GLMM vs GEE](https://github.com/younghhk/MM)

Comparison of mixed-effects models vs GEE for clustered and longitudinal epidemiologic data.

---
##  Nutritional Epidemiology & Diet Quality 🥗

### [Healthy Eating Index (HEI) Software](https://github.com/younghhk/HEI)

R-based implementation of **HEI-2020** using NHANES and FPED, following USDA/NCI scoring methodology.

### [IDATA Metabolomics Project](https://github.com/younghhk/IDATA)

Metabolomics analyses from the **IDATA** biomarker validation study evaluating diet and activity reporting.

🔒 Access restricted to authorized collaborators.

---
##  Causal & Mediation Methods 🔗

### [Planning Mediation Analysis](https://github.com/younghhk/Mediation-Analysis)

Framework for selecting appropriate mediation analysis strategies in observational cancer research.

### [High-Dimensional Mediation Analysis](https://github.com/younghhk/Moore)

Mediation methods tailored for high-dimensional omics data such as methylation and gene expression.

🔒 Access restricted to authorized collaborators.


---
##  Meta-Analysis & Evidence Synthesis 📊

### [Meta-Analysis for Clinical Research](https://github.com/younghhk/Meta-Analysis)

Key concepts, formulas, and methods for fixed-effect and random-effects meta-analysis.

---
##  Survival Analysis & Methods Development  📉 

### [Delayed Entry in Cox Models](https://github.com/younghhk/Survival-Analysis#sec-time-scale-delayed-entry)

Handling left truncation and aligning study entry times.

### [Adjusted Survival Curves](https://github.com/younghhk/Survival-Analysis#sec-adjusted-survival)

Estimating covariate-adjusted survival curves from Cox models.

### [Survival Prediction Using Machine Learning](https://github.com/younghhk/Survival-Analysis#survival-prediction-using-machine-learning)

Applications of RSF, neural networks, and boosting for risk prediction.

### [Biomarker Identification for Survival](https://academic.oup.com/pcm/article/2/2/90/5520072)

Identifying CpGs and molecular markers associated with short or long cancer survival.

---
##  Health Disparities & Decomposition Methods ⚖️

### [Peters–Belson Decomposition](https://github.com/younghhk/Disparity-Decomposition#petersbelson-decomposition-on-the-proportion-of-death-black-vs-white)

Quantifying survival disparities explained by measurable vs residual factors.

### [Quantile-Based Decomposition](https://pmc.ncbi.nlm.nih.gov/articles/PMC12456447/)

Distributional disparity analyses for complex survey data.

### [Longitudinal Disparity Decomposition](https://doi.org/10.10093/biostatistics/kxaf044)

Evaluating disparities that evolve over follow-up.

---
##  Quantile Methods in Cancer Research 📈

* Demographic associations with leukocyte telomere length (in revision)
* [CpG associations with short vs long cancer survival](https://academic.oup.com/pcm/article/2/2/90/5520072)
* Distributional analyses of racial/ethnic disparities in breast cancer survival

--- 
##  High-Dimensional Statistical Learning 🧠

### [Variable Selection & Stability](https://github.com/younghhk/VS)

High-dimensional biomarker selection using LASSO, Elastic Net, Group LASSO, and Stability Selection.

### Recent Methodological Work

* Genetic effects in longitudinal phenotypes (2025)
* Quantile forward regression for survival (2023)
* KNN–LASSO regional quantile modeling (2023)
* Conditional quantile inference for censored data (2023)

### Earlier Developments

(Feature screening, ultrahigh-dimensional LDA, IPOD, sequential GLMs, etc.)

---
##  Radiation Epidemiology ☢️

### [Radiation Epidemiology Risk Modeling in R](https://github.com/younghhk/Radiation-epi)

Overview of **Colossus** and **Epicure** for dose–response modeling, survival analysis, and radiation risk estimation.


---
##  Clinical Trials Methods 🔬

### [Training Resources](https://github.com/younghhk/ClinicalTrials)

Materials on clinical trial design, power, sample size, and key methodological principles.

---
##  Datasets & Codebooks 📁

### [NHANES](https://github.com/younghhk/NHANES)

Documentation, variable descriptions, and examples for the National Health and Nutrition Examination Survey.

---


# 👤 Author

**Hyokyoung "Grace" Hong**
📧 [grace.hong@nih.gov](mailto:grace.hong@nih.gov)

Senior Investigator </br>
Biostatistics Branch </br>
Division of Cancer Epidemiology and Genetics </br>
National Cancer Institute </br>
National Institutes of Health </br>


