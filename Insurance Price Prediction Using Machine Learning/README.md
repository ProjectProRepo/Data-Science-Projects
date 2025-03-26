# Insurance Pricing Forecast Using XGBoost Regressor

## Overview
This project focuses on building a machine learning model to predict insurance pricing using linear regression and XGBoost regression techniques. Insurance companies rely on accurate forecasting models to set premium rates that balance profitability and customer affordability. 
We explore key features such as age, BMI, smoking status, and region to determine healthcare charges. The project includes exploratory data analysis, correlation analysis, regression model building, and hyperparameter tuning for optimal results.

## Dataset
The dataset consists of 1,338 records of insured customers, containing key attributes such as:
- **age**: Age of the primary beneficiary.
- **sex**: Gender of the primary beneficiary.
- **BMI**: Body Mass Index of the beneficiary.
- **children**: Number of dependent children.
- **smoker**: Whether the primary beneficiary smokes.
- **region**: Residential area in the US.
- **charges**: Individual medical costs billed by health insurance.

## Tech Stack
- **Programming Language**: Python
- **Libraries**: `pandas`, `numpy`, `matplotlib`, `plotly`, `statsmodels`, `sklearn`, `xgboost`, `skopt`

## Project Workflow
### 1. Exploratory Data Analysis (EDA)
- **Univariate Analysis**: Distributions of continuous and categorical variables.
- **Bivariate Analysis**: Identifying relationships between independent variables and insurance charges.
- **Correlation Analysis**:
  - Pearson Correlation (for numerical variables)
  - Chi-squared Tests (for categorical variables)
  - ANOVA (Analysis of Variance for categorical-target relationships)

### 2.Baseline Model: Linear Regression
- Understanding assumptions of linear regression.
- Performing data preprocessing.
- Training the model.
- Evaluating performance using RMSE.

### 3.XGBoost Regressor Model
- Introduction to XGBoost and why it is helpful for this problem.
- Implementing `Pipeline` from `sklearn` to streamline preprocessing and model training.
- Hyperparameter tuning is performed using BayesSearchCV.
- Model evaluation using RMSE.

### 4. Model Comparison & Insights
- Comparing Linear Regression** vs. XGBoost Regressor.
- Understanding feature importance.
- Communicating results effectively to non-technical stakeholders.

## Expected Outcomes
By completing this project, users will:
- Understand insurance pricing models and key influencing factors.
- Build and evaluate linear and XGBoost regression models.
- Optimize models using hyperparameter tuning.
- Learn how to interpret and present results effectively.

## Learning Takeaways
- Exploratory Data Analysis (EDA) techniques for regression problems.
- Feature selection and engineering for regression models.
- Understanding and validating linear regression assumptions.
- Implementing XGBoost for regression.
- Using `sklearn.Pipeline` for efficient model building.
- Applying Bayesian Optimization (`BayesSearchCV`) for hyperparameter tuning.

## Hands-On Solution Code
[Insurance Price Prediction Data Science Project Solution Code](https://www.projectpro.io/project-use-case/insurance-pricing-forecast-using-regression-analysis)
