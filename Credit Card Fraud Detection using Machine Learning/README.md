# Credit Card Fraud Detection Data Science Project

## Overview
This project focuses on building a machine learning model to detect fraudulent credit card transactions. With financial fraud becoming increasingly sophisticated, this project aims to build a robust classification model that can differentiate between genuine and fraudulent transactions. The dataset used is highly imbalanced, requiring careful handling of class distribution to improve prediction accuracy.

## Dataset
**Source:** The dataset consists of transactions made by European credit cardholders in September 2013, collected as part of a research collaboration between Worldline and the Machine Learning Group at Université Libre de Bruxelles (ULB).

**Key Attributes:**
- **Time:** Seconds elapsed between the first transaction and the current transaction.
- **Amount:** Transaction amount.
- **V1 - V28:** Anonymized features resulting from PCA transformation.
- **Class:** Target variable (0: Non-Fraud, 1: Fraud).

**Dataset Characteristics:**
- **Total Transactions:** 284,807
- **Fraudulent Transactions:** 492 (~0.172%)
- **Imbalance Ratio:** Highly skewed towards non-fraudulent transactions

## Tech Stack
- **Programming Language:** Python 3.10.4
- **Libraries:**
  - `numpy`, `pandas` - Data manipulation
  - `matplotlib`, `seaborn` - Data visualization
  - `scikit-learn` - Machine learning models and preprocessing
  - `imbalanced-learn` - Handling class imbalance

## Project Workflow
1. **Understanding the Problem**
   - Define business impact and key challenges
   
2. **Exploratory Data Analysis (EDA)**
   - Understanding dataset structure
   - Visualizing data distributions and correlations
   - Identifying outliers using boxplots and interquartile range
   
3. **Data Preprocessing**
   - Handling missing values
   - Feature scaling
   - Converting categorical features (if any)
   
4. **Dealing with Class Imbalance**
   - **Undersampling:** NearMiss technique
   - **Oversampling:** SMOTE (Synthetic Minority Over-sampling Technique)
   
5. **Building Machine Learning Models**
   - **Baseline Model:** Random Forest Classifier
   - **Logistic Regression:** Interpretable model
   - **Ensemble Techniques:** Random Forest for improved generalization
   - **Non-Linear Models:** SVM, Decision Tree, k-Nearest Neighbors
   
6. **Model Evaluation & Validation**
   - Cross-validation for robust performance assessment
   - Metrics: Accuracy, Precision, Recall, F1-score
   - ROC Curve & AUC for evaluating class separation
   - Learning curves for model behavior analysis
   
7. **Model Selection & Deployment Considerations**
   - Comparison of models based on key metrics
   - Selecting the most optimal model for production use

## Expected Outcomes
- A trained classification model that effectively detects fraudulent transactions.
- Insights into the effectiveness of handling imbalanced datasets.
- A comparative analysis of different classification algorithms.
- Visualization of fraud detection performance through various evaluation metrics.

## Learning Takeaways
- Understanding imbalanced data problems and techniques to address them.
- Applying feature scaling and outlier detection methods.
- Implementing various classification models using `scikit-learn`.
- Evaluating model performance using appropriate metrics for fraud detection.
- Learning the importance of Recall over Accuracy in imbalanced datasets.
- Applying hyperparameter tuning techniques like GridSearchCV and RandomSearchCV.

## Hands-On Solution Code
Access the complete solution code with documentation for the [Fraud Detection Project
](https://www.projectpro.io/project-use-case/credit-card-fraud-detection-classification-problem)
