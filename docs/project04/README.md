# Project 4 - Predicting a Continuous Target with Regression (Titanic)

## Author: Houston Asher-Laws

## November 16th 2025

In this project instead of predicating class like survied we will predict fare and the amount of money paid for the journey.

## Section 1 — Import & Inspect the Data

Loaded the Titanic dataset using Seaborn and inspected the first few rows to confirm structure and identify important columns. Verified that fare is a continuous numeric target appropriate for regression.

## Section 2 — Data Exploration & Preparation

Handled missing values for age, removed rows missing fare, and created new features such as family_size. Converted categorical features (like sex) into numeric form when used in modeling. Ensured the dataset was clean and ready for regression.

## Section 3 — Feature Selection

Built four different feature sets (Cases 1–4) to test how different combinations of inputs predict fare.

Case 1: age

Case 2: family_size

Case 3: age + family_size

Case 4: sex + pclass (best case)
Explained why each feature might matter for predicting ticket cost.

## Section 4 — Linear Regression Modeling

Trained linear regression models on all four cases and evaluated performance using R², RMSE, and MAE. Compared training vs. testing results to determine underfitting or overfitting. Identified Case 4 (sex + pclass) as the best-performing feature combination.

## Section 5 — Alternative Models (Ridge, Elastic Net, Polynomial)

Applied regularization to the best case:

Ridge: similar performance to linear regression

Elastic Net: best overall model
Also tested polynomial regression on a single-feature case (family_size). Higher-degree polynomials didn’t improve predictions because the feature had weak correlation with fare.

