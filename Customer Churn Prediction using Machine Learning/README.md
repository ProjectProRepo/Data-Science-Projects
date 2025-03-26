# Churn Prediction Model using Ensemble Learning

## Overview
This project focuses on building an ensemble learning-based machine learning model to predict customer churn. The goal is to determine whether a customer will renew their subscription or discontinue the service. We implement and compare different ensemble methods such as Random Forest, AdaBoost, and Gradient Boosting to improve predictive performance. 

## Dataset
The dataset provides information about a video streaming service company aiming to predict customer churn. It consists of approximately 2000 rows and 16 columns, including key customer attributes such as:
- Customer tenure
- Monthly charges
- Subscription type
- Usage patterns
- Customer support interactions
- Churn status (Target variable)

## Tech Stack
- **Language**: Python
- **Libraries**: NumPy, pandas, matplotlib, scikit-learn, pickle, imbalanced-learn (SMOTE), LIME

## Project Workflow
1. **Data Exploration & Preprocessing**
   - Load dataset and inspect structure
   - Handle missing values
   - Perform exploratory data analysis (EDA)
   - Feature engineering (dropping unnecessary columns, encoding categorical variables)
   
2. **Data Splitting**
   - Split dataset into training and testing sets
   - Handle imbalanced data using SMOTE

3. **Model Building**
   - Implement Random Forest
   - Implement AdaBoost
   - Implement Gradient Boosting

4. **Model Evaluation**
   - Compute Accuracy, Precision, Recall, and F1-score
   - Evaluate models using ROC and AUC curves
   - Analyze feature importance

5. **LIME Interpretation**
   - Use LIME (Local Interpretable Model-agnostic Explanations) to explain model predictions

## Expected Outcomes
- A well-performing machine learning model that predicts customer churn.
- Identification of key factors influencing customer churn.
- Implementation of ensemble learning techniques for improved model accuracy.
- Hands-on experience with feature selection, model evaluation, and interpretability techniques.

## Learning Takeaways
- Understanding ensemble learning (Bagging vs. Boosting)
- Working with Random Forest, AdaBoost, and Gradient Boosting models
- Data preprocessing and feature engineering for machine learning
- Handling imbalanced datasets with SMOTE
- Model evaluation using performance metrics
- Interpreting model predictions using LIME

## Hands-On Solution Code
[Customer Churn Prediction Data Science Project](https://www.projectpro.io/project-use-case/how-to-build-a-churn-prediction-model-using-ensemble-learning)
