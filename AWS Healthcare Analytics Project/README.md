# End-to-End Snowflake Healthcare Analytics Project on AWS

## Overview

This project leverages Snowflake on AWS to predict patient length of stay (LOS) in hospitals. Predicting LOS helps with resource allocation, reducing infection risks, and optimizing hospital operations. Using machine learning algorithms, we analyze patient admission data stored in Snowflake to make accurate predictions, integrating AWS SageMaker for model training and deployment.

## Dataset

- **Source:** Hospital patient admission records (simulated or real-world dataset)
- **Key Attributes:**
  - Patient demographics
  - Admission details (date, department, severity)
  - Previous medical history
  - Lab test results
  - Discharge status
  - Length of stay (target variable)

## Tech Stack

- **Tools:** AWS SageMaker, Snowflake
- **Language:** Python
- **Libraries:**
  - `snowflake-connector-python`, `snowflake-sqlalchemy`
  - `xgboost`, `pandas`, `numpy`, `scikit-learn`

## Project Workflow

1. **Understanding Snowflake UI** - Working with worksheets, dashboards, and queries.
2. **Exploratory Data Analysis (EDA) in Snowflake** - Analyzing patient admission data.
3. **Feature Engineering in Snowflake** - Creating new features to improve prediction accuracy.
4. **AWS SageMaker Setup** - Configuring instances and integrating with Snowflake.
5. **Fetching Data from Snowflake** - Using Python connectors (`snowflake-connector-python`).
6. **Data Preprocessing** - Handling missing values, encoding categorical data.
7. **Feature Selection** - Using correlation analysis, statistical tests.
8. **Model Building**:
   - **Linear Regression**
   - **Random Forest Regression**
   - **XGBoost Regression**
9. **Model Predictions** - Generating predictions on new patient data.
10. **Inserting Model Predictions in Snowflake** - Storing results in a dedicated logging table.
11. **Scoring Function Deployment** - Automating predictions with scheduled jobs.
12. **Sending Status Emails** - Notifying stakeholders of model execution status.

## Expected Outcomes

- **Accurate predictions** of patient length of stay.
- **Efficient resource planning** for hospital management.
- **Improved patient care** through better forecasting.
- **Hands-on experience** integrating Snowflake with AWS SageMaker.

## Learning Takeaways

- How to use Snowflake for data warehousing and analytics.
- Feature engineering and selection for healthcare analytics.
- Building and evaluating regression models for LOS prediction.
- Deploying models in AWS SageMaker.
- Automating machine learning workflows with Snowflake and Python.

## Hands-On Solution Code
[End-to-End Healthcare Analytics Project -Part 1](https://www.projectpro.io/project-use-case/snowflake-healthcare-analytics-project)

[End-to-End Healthcare Analytics Project -Part 2](https://www.projectpro.io/project-use-case/aws-sagemaker-healthcare-analytics-project)
