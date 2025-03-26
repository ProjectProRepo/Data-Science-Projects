# Loan Eligibility Prediction using Gradient Boosting Classifier

## Overview
This data science project aims to predict whether a loan should be granted to an applicant based on various factors such as credit score and past financial history. The goal is to automate the loan approval process for SYL Bank, one of Australia's largest banks, which currently processes applications manually. By leveraging machine learning, we can develop a robust classification model to assist in making data-driven decisions.

## Dataset
The dataset consists of historical loan application records with key attributes such as:
- **Applicant Income**: Monthly income of the applicant.
- **Co-applicant Income**: Monthly income of the co-applicant (if any).
- **Loan Amount**: The amount of loan requested.
- **Loan Amount Term**: Duration of the loan in months.
- **Credit History**: Applicant's history of repaying debts.
- **Marital Status**: Whether the applicant is married or single.
- **Education Level**: The applicant’s educational background.
- **Self-Employed**: Whether the applicant is self-employed or salaried.
- **Property Area**: The area where the applicant’s property is located (Urban/Rural/Semiurban).
- **Loan Status**: Target variable indicating whether the loan was approved or not.

## Tech Stack
- **Programming Language**: Python
- **Libraries Used**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Imbalanced-learn (SMOTE), Pickle

## Project Workflow
1. **Understanding the Business Problem**
   - Identifying key factors influencing loan eligibility.
   - Defining business objectives and expected outcomes.

2. **Exploratory Data Analysis (EDA)**
   - Analyzing categorical and numerical features.
   - Handling missing values and outliers.
   - Feature engineering and encoding categorical variables.

3. **Data Preprocessing**
   - Handling missing values using imputation techniques.
   - Normalizing and transforming data for better model performance.
   - Balancing the dataset using SMOTE (Synthetic Minority Over-sampling Technique).

4. **Model Building**
   - Implementing baseline classification models.
   - Training a Gradient Boosting Classifier.
   - Comparing results with other models like XGBoost.
   
5. **Model Evaluation**
   - Using Cross-Validation for reliable performance metrics.
   - Evaluating models based on ROC Curve, MCC Score, and Accuracy.
   
6. **Deployment and Automation**
   - Saving trained models using Pickle for future use.
   - Scheduling ML jobs for automated loan approval processing.

## Expected Outcomes
- A machine learning model capable of predicting loan eligibility with high accuracy.
- An automated decision-making system reducing manual processing time.
- Improved fairness and transparency in loan approval decisions.
- A deployable solution with reusable model artifacts.

## Learning Takeaways
- Understanding how to approach a classification problem in machine learning.
- Conducting in-depth exploratory data analysis and feature engineering.
- Handling imbalanced datasets using SMOTE.
- Implementing and tuning Gradient Boosting Classifier for optimal performance.
- Understanding key machine learning model evaluation metrics such as ROC Curve, MCC Score, and Accuracy.
- Saving and deploying machine learning models for real-world applications.

## Hands-On Solution Code
[Loan Eligibility Prediction using Machine Learning](https://www.projectpro.io/project-use-case/loan-prediction-analytics)
