---
layout: page
title: Predicting 10-Year Coronary Heart Disease Risk
description: Machine learning on Framingham Heart Study data, and a lesson in resampling
importance: 3
category: coursework
---

**Question.** How well do machine learning models predict 10-year coronary heart disease risk in the Framingham Heart Study (n = 4,240)?

**Methods.** In R, I compared KNN, random forest, and XGBoost models, using SMOTE to address class imbalance and stratified train/test splits to prevent data leakage.

**Findings.** XGBoost dropped 0.29 in AUC between cross-validation and the held-out test set. I traced this to the distributional shift created by SMOTE-balanced training folds, which led to recommendations against improper resampling practices.

*May 2026*
