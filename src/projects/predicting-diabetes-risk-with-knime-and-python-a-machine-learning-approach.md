---
title: "Predicting Diabetes Risk with Knime and Python: A Machine Learning Approach"
emoji: 🧪
date: 2024-10-27T16:59:33.310Z
summary: "Predicting Diabetes Risk with Knime and Python: A Machine Learning Approach"
metaDescription: "Predicting Diabetes Risk with Knime and Python: A Machine Learning Approach"
tags:
  - KNIME
  - ML
  - python
---
In this project, we leveraged Knime and Python to build a classifier predicting diabetes risk using the BRFSS (Behavioral Risk Factor Surveillance System) dataset. With 40,108 records and 18 variables covering health-related risk factors, the dataset enabled us to examine various patient attributes, from BMI and physical activity to hypertension and diet.

Our workflow included data pre-processing in Knime, where we handled outliers and feature selection to refine the model. Using Random Forests and Cfs Subset Evaluator, we identified eight key predictors, including BMI, general health, and cholesterol checks. After partitioning the data into training and test sets, we tested several classifiers, ultimately selecting the J48 decision tree model for its balanced performance.

The final model achieved an accuracy of 71.9% and an AUC of 0.754, providing a reliable basis for diabetes risk prediction. To showcase the findings, we developed a Knime Data App, creating a user-friendly interface for data exploration and visualization, making the analysis accessible for healthcare professionals and general users alike. This project highlights the power of Knime’s visual workflows and Python’s analytical flexibility in tackling health-related classification challenges.

![knime logo](/src/assets/img/knime.jpeg "knime")