# MedDatathon-2026 - Predicting Heart Disease Severity with Machine Learning

## Overview
Heart disease is one of the leading causes of mortality worldwide. Early identification of high-risk patients can enable preventive interventions and reduce long-term cardiovascular complications.

This project explores whether machine learning models can predict heart disease severity using patient clinical indicators such as age, cholesterol level, resting blood pressure, and exercise test results.

## Team Members (Alphabetical by Last Name):
- Xuyang Chen
- Xinghao Huang
- Kaiyue Wang
- Yiwen Wang
- Junyi Yao
- Boyi Zhang

## Dataset
We use the **UCI Heart Disease dataset** from Kaggle:

https://www.kaggle.com/datasets/redwankarimsony/heart-disease-data

The dataset includes clinical indicators such as age, cholesterol level, blood pressure, chest pain type, and exercise test results, which are commonly used to study heart disease prediction.

## Exploratory Data Analysis

Key observations:

- Age distribution shifts toward higher values as disease severity increases.

- Maximum heart rate decreases with age.

- Higher ST depression values appear more frequently in severe cases.

- Most variables show weak correlations, suggesting low multicollinearity.

## Models:
We compared several models:

- Dummy Classifier (baseline)

- Logistic Regression

- Random Forest

- XGBoost

- LightGBM

Due to class imbalance, Macro F1 score was used as the primary evaluation metric.

## Results

- Logistic Regression already captured useful patterns (Macro F1 ≈ 0.64).

- Tree-based models improved performance.

- Tuned LightGBM achieved the best overall performance.

Model interpretation using SHAP showed that important predictors include:

- ST depression (oldpeak)

- chest pain type

- age

- exercise-induced angina
