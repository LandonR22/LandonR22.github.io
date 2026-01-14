---
title: "A Reproducibility Study of Feature Selection and Boosted Classifiers"
summary: "A reproducibility study evaluating feature selection and boosted classification models across healthcare and agricultural datasets, with a focus on robustness, overfitting, and generalizability."
tags:
  - Machine Learning
  - Reproducibility
  - Feature Selection
  - Classification
  - Python
  - Data Science
date: ''
---

## Overview
This project reproduced and critically evaluated a published machine learning study that reported near-perfect performance in predicting Chronic Kidney Disease (CKD) using feature selection and boosted classifiers. The goal was to assess whether the original findings were reproducible, robust, and generalizable when applied to contemporary datasets with different characteristics. This project was conducted as a collaborative group study as part of UCL’s *Machine Learning for Data Science* coursework, with contributions spanning data preparation, methodological implementation, and results analysis.

In addition to the original CKD dataset, the methodology was extended to two modern datasets — thyroid cancer recurrence and rice species classification — to evaluate model behavior under varying conditions of data size, class balance, and feature dimensionality.

---

## Project Output
{{< icon name="download" pack="fas" >}}
{{< staticref "uploads/CEGE0004_Final_Report_LLR3_updated.pdf" "newtab" >}}
View full project report (PDF)
{{< /staticref >}}

---

## Methods
The analysis followed a structured reproducibility and validation workflow:

- Reconstructed the original study’s methodology using Scikit-learn due to missing code and undocumented preprocessing steps
- Cleaned and preprocessed multiple datasets, including:
  - Imputation of missing values
  - Encoding categorical variables
  - Feature scaling
- Applied **Information Gain (IG)** for feature selection using:
  - The original study’s arbitrary threshold
  - A more systematic standard-deviation-based threshold
- Implemented and tuned classification models:
  - Logistic Regression (LR)
  - Decision Tree (DT)
  - Support Vector Machine (SVM)
- Applied **AdaBoost** to each base classifier
- Performed 5-fold cross-validation with grid search hyperparameter tuning
- Evaluated performance using accuracy, precision, sensitivity, F-measure, and ROC–AUC metrics

---

## Key Results
- Successfully reproduced the original study’s results on the CKD dataset, including **perfect performance from AdaBoost–Decision Trees**
- Found that boosting consistently improved **tree-based models**, but often degraded performance for **linear models** (Logistic Regression), especially on small or imbalanced datasets
- Demonstrated that feature selection can either improve or harm performance depending on dataset structure and model choice
- Identified overfitting and instability in boosted linear models when applied to modern datasets
- Highlighted that model performance is strongly influenced by:
  - Dataset size
  - Class imbalance
  - Feature dimensionality
  - Algorithm sensitivity to noise

Overall, the study emphasized that high reported accuracy alone is insufficient without transparency, reproducibility, and testing across diverse data contexts.

---

## Tools & Skills
Python · Scikit-learn · Feature Selection · Ensemble Learning · Model Evaluation · Cross-Validation · Reproducible Research · Data Preprocessing · Statistical Metrics
