Project 3 – Building a Classifier (Titanic Survival Prediction)

Author: Houston Asher-Laws
Date: November 9th 2025


This project builds and compares three machine learning classifiers — Decision Tree, Support Vector Machine (SVC), and Neural Network (MLPClassifier) — using the Titanic dataset.
The goal is to predict passenger survival based on selected input features and evaluate each model’s performance.

Objectives

Prepare and clean the Titanic dataset for modeling.

Build and evaluate classifiers using different input feature sets.

Compare performance across three model types.

Reflect on insights, accuracy, and predictive features.

Feature Cases
case	features	description
1	alone	binary feature showing if the passenger traveled alone
2	age	continuous feature representing passenger age
3	age, family_size	combined numeric features representing social and family factors
Models Used
model	description
Decision Tree (DT)	splits data into rules; easy to interpret but may overfit
Support Vector Machine (SVC)	finds the best boundary (hyperplane) between classes
Neural Network (NN)	learns complex, non-linear relationships using hidden layers
Key Findings
case	model	performance	insights
1	decision tree	simple and interpretable, single split	“alone” feature separated survivors effectively
2	decision tree	deeper tree, more complex	“age” added detail but risked overfitting
3	decision tree	best of DTs, balanced accuracy	younger and smaller families had higher survival
3	svc	performed well with clear separation	two features improved boundary definition
3	neural network	best overall	captured non-linear survival patterns clearly
Challenges Faced

Initial convergence issues with SVC support vectors.

Neural network tuning required higher iteration counts.

Needed troubleshooting to ensure correct model visualization.

Next Steps

Experiment with more complex neural networks (more layers or activation functions).

Add additional Titanic features (e.g., sex, class, fare) to improve accuracy.

Compare model performance using cross-validation and scaling methods.