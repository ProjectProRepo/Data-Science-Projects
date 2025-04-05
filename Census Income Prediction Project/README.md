# Adult Census Income Prediction

Predict whether a person earns more than \$50K/year using demographic and socioeconomic data from the 1994 U.S. Census. This project demonstrates a complete data science pipeline, from exploratory analysis to model evaluation using deep learning and classical ML techniques.

---

## Overview

This project uses the Adult Income Dataset to predict whether an individual's income exceeds \$50,000 annually. The goal is to build robust classification models using machine learning algorithms and deep neural networks. Key aspects of the project include:

- Comprehensive exploratory data analysis (EDA)
- Data preprocessing and feature engineering
- Model development using Deep Neural Networks (DNN)
- Evaluation using metrics like Accuracy, Precision, Recall, F1-score, and AUC
- Addressing class imbalance and overfitting issues

---

## Dataset

- **Source:** [UCI Machine Learning Repository - Adult Data Set](https://archive.ics.uci.edu/ml/datasets/adult)
- **Rows:** 48,842
- **Columns:** 15 (14 features + 1 target)
- **Target Variable:** `income` (`>50K`, `<=50K`)
- **Imbalanced Dataset:**
  - `>50K`: ~25%
  - `<=50K`: ~75%

### Key Attributes

- `age`: Age of the individual
- `workclass`: Type of employment (Private, Self-emp, Govt.)
- `education`: Highest education level
- `marital-status`: Marital status
- `occupation`: Occupation type
- `race`, `sex`: Demographic data
- `capital-gain`, `capital-loss`: Financial gains/losses
- `hours-per-week`: Weekly working hours
- `native-country`: Country of origin

---

## Tech Stack

- **Languages:** Python
- **Libraries & Frameworks:**
  - `pandas`, `numpy` – Data manipulation
  - `matplotlib`, `seaborn` – Data visualization
  - `scikit-learn` – ML modeling and evaluation
  - `tensorflow`, `keras` – Deep learning (Vanilla DNN)
  - `h2o.ai` – Distributed ML modeling (for scalability and experimentation)

---

## Project Workflow

### 1. Problem Understanding
- Understand business context and real-world applications of income prediction.

### 2. Data Loading & Inspection
- Load CSV data
- Check missing values, data types, and basic statistics

### 3. Exploratory Data Analysis (EDA)
- Univariate and bivariate visualizations
- Distribution checks and outlier analysis
- Class imbalance check

### 4. Data Preprocessing
- Convert `?` to NaN and handle missing values
- Encode categorical features (Label Encoding, One-hot Encoding)
- Normalize/scale numeric variables
- Stratified train-test split to preserve class ratio

### 5. Feature Engineering
- Feature transformation and binning
- Derived features from existing variables

### 6. Model Development
- Train a **Vanilla DNN** using Keras
- Try alternate architectures for improved performance

### 7. Model Evaluation
- Evaluate with:
  - Accuracy
  - Precision
  - Recall
  - F1 Score
  - ROC-AUC
- Understand when **Accuracy** is not enough due to class imbalance

### 8. Hyperparameter Tuning
- Cross-validation to assess overfitting
- Hyperparameter tuning for DNN and ML models

### 9. Model Selection
- Choose the best model based on evaluation metrics and feature importance

---

## Expected Outcomes

- A trained classification model that can predict income levels based on demographic and economic variables
- Clear understanding of the role of data preprocessing, EDA, and model evaluation
- Deployable code for similar binary classification problems

---

## Learning Takeaways

- Understanding of end-to-end data science project lifecycle
- Handling class imbalance in datasets
- Feature encoding and engineering best practices
- Building and tuning deep learning models
- Model evaluation techniques and metric selection
- Use of H2O.ai for scalable model experimentation

---

## Hands-On Solution Code
[
Census Income Prediction Data Science Project](https://www.projectpro.io/project-use-case/census-income-dataset-project)

---

## Use Cases of Census Income Data

- **Marketing**: Customer segmentation and targeting by income level
- **Credit Risk**: Loan eligibility and credit scoring
- **Healthcare**: Accessibility analysis in low-income regions
- **Real Estate**: Identifying areas for luxury or budget housing
- **Education & Non-Profits**: Program targeting in underserved regions

