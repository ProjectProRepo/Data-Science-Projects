# Credit Card Default Prediction using Machine Learning

## Overview
This project aims to predict the likelihood of borrowers defaulting on credit loans by building a **credit score prediction model**. It leverages machine learning techniques to analyze borrowers' profiles and historical credit records. By accurately identifying potential defaulters, financial institutions can take proactive measures to minimize risk and improve loan management strategies.

## Business Context
Banks generate revenue by lending money while ensuring timely repayments. Identifying borrowers who are likely to default helps banks take preventive measures, such as sending reminders or adjusting credit policies. This project focuses on predicting **serious delinquency**—cases where a borrower is behind on payments for more than three months—over the next two years.

## Dataset
The dataset used in this project consists of **training and test data files**, containing both **general profile attributes** (age, income, dependents) and **historical credit behavior** (debt ratio, credit utilization, past defaults). 

Key Attributes:
- **Age**: Borrower's age
- **Monthly Income**: Salary or earnings per month
- **Dependents**: Number of dependents
- **Debt Ratio**: Ratio of monthly debt payments to income
- **Past Defaults**: Number of times the borrower has defaulted in the past
- **Credit Utilization**: Ratio of used credit to the total credit limit

## Tech Stack
This project is implemented in **Python 3.8** and uses the following libraries:

- **Pandas**: Data manipulation and aggregation
- **NumPy**: Efficient numerical computations
- **Matplotlib & Seaborn**: Data visualization
- **Scikit-Learn**: Model training, optimization, and evaluation
- **Imbalanced-Learn**: Handling class imbalance issues
- **Shap & LIME**: Model interpretability
- **Keras**: Deep learning model implementation

## Project Workflow
1. **Data Preprocessing**
   - Handling missing values
   - Treating outliers
   - Stratified sampling
   - Feature scaling (Box-Cox transformation, standardization)

2. **Exploratory Data Analysis (EDA)**
   - **Univariate & Bivariate Analysis**: Understanding distributions and relationships
   - **Event Rate Calculation**: Determining default rates for different segments

3. **Feature Engineering**
   - Upsampling & Downsampling for handling class imbalance
   - Recursive Feature Elimination (RFE) using Cross-Validation

4. **Model Building**
   - **Logistic Regression**
   - **Neural Networks (Deep Learning)**
   - **Tree-based Models (Random Forest, XGBoost, Bagging, Boosting)**

5. **Model Optimization**
   - Hyperparameter tuning using Grid Search & Random Search
   - Performance evaluation: **F1 Score, Precision, Recall, AUC-ROC Curve**

6. **Model Interpretability**
   - **SHAP (Global Level Interpretability)**
   - **LIME (Local Level Interpretability)**

7. **Results & Insights**
   - Comparing different models' performances
   - Business implications of model predictions

## Expected Outcomes
By the end of this project, users will:
- Understand key **credit risk factors** influencing loan defaults
- Learn **data preprocessing techniques** for financial datasets
- Build and evaluate **machine learning models** for credit risk assessment
- Gain experience in **model interpretability tools (SHAP, LIME)**

## Learning Takeaways
- Handling **class imbalance** using **upsampling, downsampling, and SMOTE**
- Feature engineering and **Recursive Feature Elimination (RFE)**
- Implementing **tree-based and deep learning models** for credit scoring
- Evaluating models using **ROC-AUC curves** and **F1 scores**
- Applying **SHAP and LIME** for explainability in financial modeling

## Hands-On Solution Code
[Credit Card Default Prediction using Machine Learning](https://www.projectpro.io/project-use-case/credit-score)
