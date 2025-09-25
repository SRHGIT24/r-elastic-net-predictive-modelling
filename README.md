# Elastic Net Predictive Modelling in R

This project demonstrates a **predictive modelling pipeline** in **R** using Elastic Net regression with post-hoc OLS correction and permutation testing.  

---

## Why Synthetic Data?
The original dataset contained **sensitive medical information** and cannot be shared publicly.  
Instead, this notebook uses a **synthetic dataset** that reproduces the same key characteristics:  
- 377 participants  
- ~7000 protein biomarkers with realistic collinearity patterns  
- Two outcomes:  
  - **BAG_std** (positive or negative, mean ~0, sd ~1)  
  - **Resilience_std** (strictly positive, sd ~1)  

The synthetic dataset was designed to mimic the statistical challenges of the real data while being completely safe to publish.

---

## Methods
The notebook implements:
1. **Elastic Net regression** (`glmnet`) with cross-validation and alpha tuning  
2. **Post-hoc OLS correction** to adjust for shrinkage bias  
3. **Permutation testing** to provide robust p-values for predictive performance  
4. **Visualisation** of model performance, feature stability, and permutation results  

---

## Tech Stack
- **Language:** R  
- **Libraries:** `glmnet`, `dplyr`, `tidyr`, `ggplot2`  

---

## Summary
This notebook provides a **blueprint for predictive modelling in high-dimensional datasets** such as omics or imaging-derived biomarkers.  
It highlights how to combine **Elastic Net, OLS correction, and permutation testing** to build a **robust and interpretable predictive pipeline**.  

---

### Disclaimer
This project uses **synthetic data only**.  
Results do not reflect real-world medical findings, but the methodology is directly transferable to sensitive datasets under proper data governance.
