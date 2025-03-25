# Insurance Claims Severity Prediction Data Science Project

## Overview
Allstate, a personal insurance company in the United States, is looking to leverage data science to predict the severity and cost of insurance claims after an unforeseen event. This project aims to:

- Build an ensemble machine learning model to predict claim severity.
- Apply best practices in data preprocessing, feature engineering, and model evaluation.
- Implement hyperparameter tuning to optimize model performance.
- Deploy the model as a Flask API for real-world applications.

## Dataset
### Source
The dataset for this project is sourced from Allstate’s insurance claim records. It consists of numerical and categorical variables representing various risk factors.

### Key Attributes
- **Claim Features:** A mix of categorical and continuous variables.
- **Target Variable:** Claim severity (continuous variable indicating claim cost).
- **Missing Values:** Some categorical and continuous features have missing data.
- **Outliers:** Certain numerical features exhibit extreme values.

## Tech Stack
- **Programming Language:** Python
- **Libraries:** `pandas`, `NumPy`, `seaborn`, `matplotlib`, `scikit-learn`, `shap`
- **Model Deployment:** Flask API

## Project Workflow
### 1️ Data Preprocessing
- Load dataset using `pandas`.
- Handle missing values for categorical and continuous variables.
- Outlier detection and treatment using box plots.

### 2️ Feature Engineering
- Label Encoding vs. One-Hot Encoding for categorical variables.
- Feature selection using correlation, constant variance, and Chi-Square statistical tests.

### 3️ Model Building
- Understand and implement ensemble machine learning algorithms (Bagging, Boosting).
- Hyperparameter tuning using `GridSearchCV` and `RandomizedSearchCV`.

### 4️ Model Evaluation
- Root Mean Squared Error (RMSE) as the evaluation metric.
- Model interpretability using SHAP values.

### 5️ Model Deployment
- Convert trained model into a `pickle` file.
- Develop and deploy a Flask API for serving predictions.

## Expected Outcomes
- A predictive model to estimate claim severity.
- A well-documented approach to data preprocessing and feature engineering.
- A Flask API for real-world integration.

## Learning Takeaways
- Hands-on experience in ensemble learning techniques.
- Advanced feature engineering and feature selection.
- Model evaluation using RMSE and SHAP.
- Deploying machine learning models with Flask.

## Hands-On Solution Code
[Insurance Claims Severity Prediction](https://www.projectpro.io/project-use-case/all-state-insurance-claims-severity-prediction)
