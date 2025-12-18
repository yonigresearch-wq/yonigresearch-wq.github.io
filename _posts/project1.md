---
title: "Rectal Cancer Survival and PDE5 Inhibitor Use"
---

<h3>Objective</h3>

To assess whether use of phosphodiesterase-5 inhibitors (PDE5Is) is associated with overall survival among male rectal cancer patients undergoing surgery, using data from Clalit Research Room (HMO database), including clinical records and pharmaceutical purchase data for approximately 1,700 patients.

---

<h3>Data Preparation and Feature Engineering</h3>

- Cleaned and validated clinical and pharmacy datasets, excluding patients who did not meet predefined inclusion criteria and removing irrelevant or unreliable variables.
- Engineered exposure variables characterizing PDE5I use from longitudinal purchase data.
- Constructed time-to-event outcomes and covariates, incorporating diagnosis timelines and most recent clinical status prior to surgery.

---

<h3>Statistical Analysis</h3>

**1. Descriptive and Exploratory Analysis**

- Compared demographic and clinical characteristics between PDE5I users and non-users using parametric and non-parametric tests.
- Created publication-quality visualizations (histograms and kernel density estimates) to assess distributional differences.

**2. Managing Potential Confounding**

- Implemented Random Survival Forests (RSF) and standardized Cox proportional hazards models to identify variables most predictive of survival.
- Evaluated model performance using Harrell’s C-index and bootstrap-based out-of-bag validation.
- Applied propensity score matching (PSM) to balance PDE5I users and non-users on key prognostic covariates, including hyperparameter tuning for both RSF and matching procedures.

**3. Survival Analysis**

- Estimated and compared survival using Cox proportional hazards models and log-rank tests in both unmatched and matched cohorts. 
- Visualized survival differences with Kaplan–Meier curves.
- Conducted subgroup analyses to explore heterogeneity of effects among PDE5I users and non-users.

---

<h3>Reporting Results</h3>

- Translated complex statistical results into clinically meaningful conclusions for non-technical medical collaborators.
- Authored a journal-style Methods and Results section, including clean tables and high-resolution figures.
- Discussed methodological limitations, potential residual confounding, and appropriate interpretation of causal claims.



