# Regression Analysis of Housing Prices

## Author: Houston Asher-Laws
## Date: November 25, 2025

This project uses Linear Regression to predict SalePrice from three features in the Ames Housing dataset:

MoSold (Month Sold)

YrSold (Year Sold)

LotArea (Lot Size)

1. Data Exploration

The dataset has 81 columns.

The three chosen features had no missing values.

I created histograms and a heatmap to understand the data.

The heatmap showed that MoSold, YrSold, and LotArea do not have a strong correlation with SalePrice.

2. Feature Selection

I used the features MoSold, YrSold, and LotArea for prediction.
The target variable is SalePrice.

3. Models Used

I tested three models:

Baseline Linear Regression

Pipeline 1: Scaler + Linear Regression

Pipeline 2: Polynomial Features (degree 3) + Scaler + Linear Regression

Pipeline 2 performed the best.

1. Results

Pipeline 2 gave better results than the baseline and the first pipeline.

Scaling alone did not change performance.

Polynomial features helped the most.

5. Challenges

Choosing only three features from the 81 columns.

Some features did not strongly relate to SalePrice.

6. Future Work

Try using more relevant features.

Test other regression models for better accuracy.