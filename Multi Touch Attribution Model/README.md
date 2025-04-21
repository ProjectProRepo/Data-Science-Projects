# Build a Multi-Touch Attribution Machine Learning Model in Python

## Overview

Understanding the **true impact of each marketing channel** on conversions is vital for **ROI optimization**. This project aims to demystify how users engage across multiple touchpoints and assigns credit to each channel using **machine learning-based attribution models**.

By the end of this project, you’ll have built a series of **Single-Touch**, **Multi-Touch**, and **Probabilistic Attribution** models in Python. You’ll also implement a **Budget Optimization Engine** that recommends how to best allocate marketing spend for maximum returns.

## Dataset

The dataset is structured in a CSV file with:
- **586,737 rows** and **6 columns**

| Column Name       | Description |
|------------------|-------------|
| `Cookie`         | Anonymous user identifier |
| `Time`           | Timestamp of user interaction |
| `Interaction`    | Type of interaction (click/view/etc.) |
| `Conversion`     | Binary flag: 1 if converted, else 0 |
| `ConversionValue`| Monetary value of the conversion |
| `Channel`        | Marketing channel name (target variable) |

## Tech Stack

- **Language**: Python 3.x
- **Environment**: Jupyter Notebook / Google Colab
- **Libraries**:
  - `NumPy`, `Pandas`, `Seaborn`, `Matplotlib`
  - `pandas-profiling` for EDA
  - `itertools`, `gekkopy` for optimization
  - Custom attribution modeling functions

## Project Workflow

### 1. Problem Understanding
- Define the objective: Measure channel-level impact on conversions.

### 2. Data Loading & Preprocessing
- Load the dataset
- Handle missing values and duplicates
- Perform time-based and user-based session segmentation

### 3. Exploratory Data Analysis (EDA)
- Generate profiling reports using `pandas-profiling`
- Understand customer journeys and conversion paths
- Analyze channel distribution and conversion timelines

### 4. Attribution Modeling

#### Single-Touch Models
- **First-Touch Attribution**
- **Last-Touch Attribution**
- **Last-Non-Direct Attribution**

#### Multi-Touch Models
- **Linear Attribution**
- **Position-Based Attribution (U-Shaped)**
- **Time Decay Attribution**

#### Probabilistic Models
- **Markov Chain Attribution**
- **Shapley Value Attribution** (using Game Theory)

### 5. Result Evaluation
- Compare model results using tables and visualizations
- Average contribution per channel
- Attribution comparison plots

### 6. Budget Optimization Engine
- Analyze performance per channel
- Recommend optimal budget allocation using Gekko optimization

## Expected Outcomes

- **Channel ROI Insights**: Understand which channels drive conversions.
- **Model Benchmarking**: Compare single vs multi-touch vs probabilistic models.
- **Budget Strategy**: Learn how to optimize marketing budgets using model-driven insights.

## Learning Takeaways

This project helps you develop skills in:

- Attribution modeling using both rule-based and probabilistic approaches
- Exploratory Data Analysis with `pandas-profiling`
- Markov Chain simulations for customer journey analysis
- Cooperative Game Theory with Shapley Values
- Optimization modeling using Gekko
- Marketing analytics using Python

## Hands-On Solution Code

[Build a Multi Touch Attribution Machine Learning Model in Python
](https://www.projectpro.io/project-use-case/multi-touch-attribution-model-python)
## Notes

- You’ll need to install `pandas-profiling`, `gekkopy`, and `networkx` for specific model implementations.
- The dataset is anonymized and structured to protect user identity.
