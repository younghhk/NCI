# SEER Cancer Data Analysis

This repository provides example code and documentation for **SEER Cancer Registry data analysis**, focusing on **incidence-based mortality (IBM) rates**, **rate ratios**, and related survival analysis methods.

> ⚠️ This repository is private. Access is restricted to approved collaborators. Please contact the owner if you need access.

---

##  Features
- Functions to compute **incidence-based mortality rates** with small-count adjustments:
  - **Fay–Feuer method** (recommended for rare events)  
  - **Tiwari’s modification** (alternative adjustment)  
- Functions to estimate **rate ratios** with variance estimates using the **delta method**  
- Example workflows demonstrating SEER-based analyses  

---

## Example Workflow

```r
# Load functions
source("IBM_functions.R")

# Example: Compute IBM rate and rate ratio
ibm_result <- compute_dsr_and_rr_for_subset(
  df,
  idx1 = which(df$Group == "Non-Hispanic White"),
  idx2 = which(df$Group == "Non-Hispanic Black"),
  label_group1 = "NHW",
  label_group2 = "NHB",
  subset_label = "Example Subset",
  ci_method = "fayfeuer"
)

print(ibm_result)
```
---

## 📄 Example PDF

An example SEER analysis is included:  
👉 [SEER_example.pdf](SEER_example.pdf)  

*(Make sure the file `seer_example.pdf` is uploaded into the repository root folder, so the link works.)*

---

## 📚 Resources
- [SEER Program Overview](https://seer.cancer.gov/)  
- [NCI Division of Cancer Epidemiology and Genetics](https://dceg.cancer.gov/)  

---

## 🔒 Repository Access

This repository is **private**.  
For access, please contact:

**Grace Hong**  
📧 [grace.hong@nih.gov](mailto:grace.hong@nih.gov)  
🔗 [GitHub Profile](https://github.com/younghhk)  
