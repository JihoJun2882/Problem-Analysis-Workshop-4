# DimensionalityReduction_Worksho
# Group Presentation 4 • README

**Course Artifact:** `DimensionalityReduction_Workshop.ipynb`  
**Prepared for:** Group 4 • Capstone Groups  
**Last updated:** 2025-11-05 05:57 UTC

This README packages everything needed to complete *Group Presentation 4* using the provided notebook. It includes a runnable checklist, deliverable templates, and an outline auto‑extracted from your Jupyter Notebook.

---

## 0) Quick Start

1. Open `DimensionalityReduction_Workshop.ipynb` in VS Code or Jupyter Lab.
2. Create/activate a Python virtual environment (suggested: Python ≥ 3.10).  
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # Windows: .venv\Scripts\activate
   pip install -U pip wheel
   ```
3. Install project deps (edit as needed):
   ```bash
   pip install numpy pandas scikit-learn scipy matplotlib ipywidgets
   ```
4. Run the notebook top‑to‑bottom. Add **Markup cells** where indicated for hypothesis testing and dimensionality‑reduction commentary.

> Tip: Keep each step reproducible. Wrap code into **classes/methods** and keep parameters centralized.

---

## 1) 100‑Word Use‑Case Update (Template)

**Context (1–2 sentences):**  
_What problem are you solving and for whom?_

**Data (1–2 sentences):**  
_What new sources did you add? What’s the target/label (if any)?_

**Method (1–2 sentences):**  
_What changed in your pipeline (feature engineering, DR, modeling)?_

**Result/Insight (1–2 sentences):**  
_What did you learn? What will you try next?_

*Aim for 95–110 words. Replace this block with your final paragraph in the notebook and paste it here.*

---

## 2) Revised Hypotheses (Unit 3 Technique)

Write these in a **Markdown cell** inside the notebook and paste here as well.

- **Null Hypothesis (H₀):** _e.g., After applying DR, model performance (AUC/MAE/etc.) does **not** improve relative to baseline._  
- **Alternative Hypothesis (H₁):** _e.g., After applying DR, model performance **does** improve relative to baseline._

Include your **test**, **metric**, **significance level (α)**, and **decision rule**.

---

## 3) Dimensionality Reduction & Feature Selection You Must Demonstrate

Add code cells (wrapped in classes/methods) and Markdown explanations for each item:

1. **Missing Values Ratio:** drop features with excessive missingness; report threshold and removed columns.  
2. **Low Variance Filter:** remove near‑constant features; report threshold and removed columns.  
3. **High Correlation Filter:** remove redundant features using a correlation matrix; justify threshold (e.g., |r| ≥ 0.9).  
4. **Principal Components Analysis (PCA):** standardize first; report explained variance ratio and how many PCs you keep.  
5. **Random Forest (Feature Importance):** rank features; discuss stability and any bias concerns.  
6. **Backward/Forward Selection:** document criteria (AIC/BIC/CV score) and final feature set.  
7. **Box‑Cox Transformation:** apply to strictly positive variables; report optimal λ and normality impact.  
8. **Tukey’s Ladder of Powers:** try several powers; compare skewness/kurtosis before vs after.

> For each technique, include: **why**, **how**, **parameters**, **before/after diagnostics** (plots + stats), and **effect on downstream task**.

---

## 4) Notebook Markup Requirements

Add clear **Markdown** sections for:
- **Hypothesis Testing:** state H₀/H₁, test, metric, α, decision, interpretation.
- **Dimensionality Reduction:** what you did and why, with before/after evidence.
- **Analysis & Discussion:** limitations, assumptions, next steps.

---

## 5) 3–5 Minute Presentation (All Team Members Speak)

- Use the notebook as your script/visuals. Keep it **tight (≤5:00 hard stop)**.  
- Suggested flow (each ~30–45s):
  1. **Problem & Data** (Speaker A)
  2. **Pipeline & DR** (Speaker B)
  3. **Results & Validation** (Speaker C)
  4. **Conclusion & Next Steps** (Speaker D)
- Keep backup slides in a final notebook section (appendix).

**Video:** Export an **MP4** using **Microsoft Clipchamp**.  
**Accessibility:** Add a **transcript** (captions).  
**Submission:** Place the **Clipchamp link** in a Markdown cell at the top of the notebook.

---

## 6) Deliverables Checklist

- [ ] Added **new data sources** and can explain them in ≤60 seconds.  
- [ ] All code **encapsulated into classes/methods**.  
- [ ] **100‑word** use‑case update written.  
- [ ] **Revised H₀/H₁** using Unit 3 technique.  
- [ ] **DR methods** implemented with diagnostics (items 1–8 above).  
- [ ] Notebook has **clear Markdown** for hypothesis testing, DR, and analysis.  
- [ ] **3–5 minute** team video (MP4) created in **Clipchamp** with **transcript**.  
- [ ] **Video link** embedded in the notebook (Markdown cell).  
- [ ] Repository contains **README + environment specs** (this file can serve as README).


## 7) Notebook Outline (Auto‑extracted)

- Retail Store Demand Forecasting
  - 1. Setup and data loading
  - 2. Data overview and basic cleaning
    - 2.1 Column description
    - 2.2 Convert date column and check missing values
  - 3. Missing values ratio
  - 4. Low variance filter
  - 5. High correlation filter
  - 6. Findings for Missing Values Ratio, Low Variance Filter, High Correlation Filter
    - 7. Principal Components Analysis (PCA)
    - Principal Components Analysis (PCA)
    - 🔍 PCA Summary — Scree Plot & Component Loadings
    - 8. Random Forest Feature Importance
    - 🌲 Random Forest Regressor — Feature Importance & Model Performance
    - ✅ Random Forest Feature Selection — Importance Threshold ≥ 0.01
    - 9. Backward and Forward Feature Selection
    - 🔍 Recursive Feature Elimination (RFE) — Selected Features
    - 10. Box–Cox Transformation
    - 11) Tukey’s Ladder of Powers
  - Video URL
