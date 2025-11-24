# Wine Quality Prediction – Ensemble Model Comparison
## Houston Asher-Laws
## Overview

This project analyzes the Wine Quality (Red) dataset and compares multiple ensemble machine learning models to determine which method best predicts wine quality based on 11 chemical features. The analysis includes data preparation, feature engineering, model training, evaluation, and final recommendations.

# 1. Data Preparation

Loaded and inspected the red wine dataset from UCI.

Created two new target columns:

quality_label → low / medium / high

quality_numeric → 0 / 1 / 2

These transformations make quality easier to classify and model.

# 2. Feature Selection

X (features): all chemical attributes, excluding quality columns

y (target): quality_numeric

This prevents target leakage and keeps only predictive variables.

# 3. Train/Test Split

Used an 80/20 split with stratification to preserve class distribution.

# 4. Models Compared

Nine ensemble methods were evaluated:

Random Forest

Gradient Boosting

AdaBoost

Bagging

Voting Classifiers

MLP Neural Network

Each model was scored using:

Train/Test Accuracy

Train/Test F1 Score

Confusion Matrix

# 5. Key Results

Random Forest (200 trees, max_depth=10) performed the best overall.

It achieved the highest Test Accuracy and Test F1, outperforming Gradient Boosting and other methods.

It showed strong generalization and handled class imbalance effectively.

6. Conclusion

Random Forest is the most reliable model for predicting wine quality in this analysis due to:

High accuracy

Strong balance between precision and recall

Good handling of nonlinear chemical interactions

Minimal overfitting compared to other models