# Avocado Price Prediction using Machine Learning

## Project Overview
This project leverages machine learning and time series forecasting techniques to predict the average price of Hass avocados in the US market. By analyzing historical sales data, we aim to provide actionable insights into market trends, enabling better strategic decision-making for avocado pricing and inventory management.

## Project Objectives
- Perform Exploratory Data Analysis (EDA) to understand the dataset
- Handle missing values and perform data preprocessing
- Engineer features, particularly time-based variables
- Visualize time-series trends and correlations
- Build and evaluate multiple forecasting models:
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
  - ARIMA & SARIMAX
- Compare model performance using evaluation metrics such as Mean Absolute Percentage Error (MAPE) and Mean Absolute Error (MAE)
- Make final price predictions based on the best-performing model
## Dataset Description
The dataset consists of weekly retail scan data of Hass avocados in the US from April 2015 to March 2018. It contains key features such as:

| Column Name       | Description |
|------------------|-------------|
| `Date`           | Observation date |
| `AveragePrice`   | Average price per avocado |
| `Type`           | Avocado type (Conventional/Organic) |
| `Region`         | Geographic region of sale |
| `Total Volume`   | Total avocados sold |
| `4046`           | Avocados sold with PLU 4046 |
| `4225`           | Avocados sold with PLU 4225 |
| `4770`           | Avocados sold with PLU 4770 |
| `Total Bags`     | Total number of bags sold |
| `Small/Large/XLarge Bags` | Number of bags sold by size |

## Tech Stack
- **Language:** Python 3.8+
- **Libraries Used:**
  - `pandas`, `numpy` – Data Manipulation
  - `matplotlib`, `seaborn` – Data Visualization
  - `statsmodels`, `pmdarima`, `fbprophet` – Time Series Analysis
  - `scikit-learn`, `xgboost` – Machine Learning Models
  
## Solution Approach

### 1) Data Preprocessing
- Handling missing values using median imputation
- Label encoding for categorical variables
- One-hot encoding for region-based features

### 2) Exploratory Data Analysis
- Trend and seasonality analysis
- Time-series decomposition
- Heatmaps for correlation analysis

### 3) Feature Engineering
- Creating lag features to capture time dependencies
- Differencing for trend elimination
- Aggregating data for better generalization

### 4) Model Building & Forecasting
- **Traditional ML Models:**
  - Linear Regression
  - Random Forest Regressor
  - XGBoost Regressor
- **Time Series Models:**
  - ARIMA
  - SARIMAX
  - Facebook Prophet

### 5) Model Evaluation
- R-squared (R²)
- Mean Absolute Percentage Error (MAPE)
- Mean Absolute Error (MAE)
- Forecast visualization with confidence intervals

## Results & Findings
- Time-series models performed better than traditional ML models for long-term forecasting.
- Facebook Prophet and ARIMA captured seasonal trends effectively.
- XGBoost Regressor provided competitive short-term predictions.
- The final model selection was based on MAPE and forecast visualization.

## Enhancements
- Incorporating external market factors such as weather conditions & import/export data
- Experimenting with LSTM & Transformer-based deep learning models for forecasting
- Extending the dataset to cover recent avocado price trends
  
## Project Solution Code
[Avocado Price Prediction using Machine Learning](https://www.projectpro.io/project-use-case/perform-time-series-modelling-facebook-prophet)

