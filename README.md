# Higher Self-Reported Mental Health Predicts Better Perceived Physical Health in Aging Adults

This repository contains the analysis code (Jupyter notebook) and supporting materials for the project:

**“Higher Self-Reported Mental Health Predicts Better Perceived Physical Health in Aging Adults”**  
Manuscript draft: *Journal of Emerging Investigators* (Manuscript Number: **JEI-26-004**)

Using the **University of Michigan National Poll on Healthy Aging (NPHA), Wave 10 (Jan–Feb 2022)** dataset (n = 2,277), we tested whether **higher self-reported mental health** predicts higher odds of reporting **“Excellent” physical health** in adults ages 50–80.

---

## Research Question

**Which factors best predict self-reported “Excellent” physical health in aging adults, and is mental health the strongest predictor?**

---

## Key Findings (from the manuscript)

- Logistic Regression (LR) produced the strongest classification performance among tested models.
- LR achieved **~77.7% accuracy** and **~78.2% F1 score** on the held-out testing set.
- **Self-reported mental health** was the strongest predictor of “Excellent” physical health.
- Physical and mental health were **moderately positively correlated** (reported r ≈ 0.29).

Top predictors identified (examples):
- Excellent mental health rating
- Higher educational attainment
- No high blood pressure/hypertension
- Higher satisfaction with social life

---

## Methods Overview

Models tested:
- Logistic Regression (LR)
- Decision Tree (DT)
- Random Forest (RF)

Workflow highlights:
- Data cleaning + encoding categorical variables
- Train/test split (80/20)
- Class imbalance handled with **SMOTE applied only to the training split** (to reduce leakage)
- Model evaluation using accuracy, precision, recall, F1 score, and ROC/AUC
- Feature importance interpretation from LR coefficients

---

## Repository Contents

- `AGING_ML_FINAL.ipynb` — primary analysis notebook (data cleaning, modeling, evaluation, visuals)

Recommended (optional) structure if you want your repo to be easy for others to run:
