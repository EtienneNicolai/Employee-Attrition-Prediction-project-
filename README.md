Employee Attrition Prediction

This project builds an end to end machine learning pipeline to predict employee attrition using structured HR data. The goal is to identify employees at risk of leaving, enabling proactive retention strategies.
Employee attrition is costly for organisations. This project frames attrition prediction as a binary classification problem:

1 = Employee leaves
0 = Employee stays

Key Features
Data preprocessing pipeline for numerical and categorical features
Missing value handling
Feature scaling and encoding
Outlier detection and removal
Class imbalance handling using SMOTE
Logistic Regression model
Adjustable classification threshold
Comprehensive evaluation metrics


Tech Stack
Python
pandas, numpy
scikit-learn
imbalanced-learn
matplotlib

Methodology
1. Data Preprocessing
Numerical features:
Median imputation
Standard scaling
Categorical features:
Most frequent imputation
One-hot encoding
2. Outlier Handling
IQR-based filtering applied to numerical features
3. Class Imbalance
SMOTE used to generate synthetic minority class samples
4. Model
Logistic Regression
Balanced class weights


6. Evaluation Metrics
Accuracy
Precision
Recall
F1 Score
Confusion Matrix


Key Insights
Class imbalance significantly impacts recall
Threshold tuning allows alignment with business priorities
Logistic regression provides a strong interpretable baseline
Limitations
Potential data leakage due to preprocessing before split
SMOTE and class weighting used simultaneously
Limited model complexity
Future Improvements
Implement full pipeline to prevent data leakage
Add cross-validation
Try advanced models (Random Forest, XGBoost)
Add model explainability (SHAP values)
Deploy as an API

I originally built this on a private dataset, but I’ve since adapted it to a public HR dataset so the pipeline is fully reproducible.
