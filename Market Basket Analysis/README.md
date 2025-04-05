# Customer Market Basket Analysis using Apriori and FPGrowth Algorithms

## Overview

This project explores **Market Basket Analysis (MBA)** using **Apriori** and **FPGrowth** algorithms. It leverages association rule learning to uncover relationships between items frequently purchased together, helping businesses improve product placement, promotions, and cross-selling strategies.

Imagine you’re a restaurant sales manager — a customer walks in and asks for a dish recommendation. Instead of guessing, you analyze purchase patterns using MBA to recommend combinations customers are more likely to enjoy. That’s exactly what this project enables using real-world retail data.

---

## Dataset

The analysis is based on an open-source dataset from a US-based convenience store chain, **FoodMart**. It comprises multiple tables that are merged and cleaned for effective analysis:

- **Customers Dataset** – Buyer information
- **Products Dataset** – Product attributes
- **Departments Dataset** – Product category info
- **Region Dataset** – Store location data
- **Sales Dataset** – Purchase history
- **Stores Dataset** – Store size and identifiers
- **Time by Day Dataset** – Timestamped transactions

These datasets are merged using common keys like `productID`, `storeID`, and `customerID` to create transaction-level item baskets.

---

## Tech Stack

- **Language:** Python  
- **Environment:** Jupyter Notebook  
- **Libraries:**  
  - `pandas`, `numpy` – Data manipulation  
  - `matplotlib`, `seaborn`, `squarify`, `networkx` – Visualization  
  - `mlxtend`, `apyori` – Association rule mining  
  - `warnings`, `gapminder` – Utilities  

- **Algorithms:**  
  - Apriori  
  - FPGrowth  

---

## Project Workflow

1. **Data Collection & Merging**
   - Import and combine datasets using shared keys.
   - Create unified transaction-level data.

2. **Data Preprocessing**
   - Handle missing values
   - Perform feature engineering
   - Create item baskets
   - One-hot encode transactions for algorithm compatibility

3. **Exploratory Data Analysis (EDA)**
   - Univariate & bivariate analysis
   - Identify top-selling products and departments
   - Visualize distribution and correlations

4. **Association Rule Mining**
   - Apply Apriori and FPGrowth algorithms
   - Configure rule parameters: support, confidence, lift
   - Filter and rank rules based on relevance

5. **Algorithm Comparison**
   - Evaluate and compare the performance (speed & memory) of Apriori vs. FPGrowth

6. **Result Interpretation**
   - Generate actionable insights
   - Recommend product pairings and shelf placements

---

## Expected Outcomes

- A list of strong **association rules** (e.g., If A is bought, B is likely to be bought)
- Visual insights on **top-selling items**, **departments**, and **basket size**
- Performance comparison of **Apriori vs. FPGrowth**
- Actionable strategies for **product bundling** and **cross-selling**

---

## Learning Takeaways

- Understand core concepts of **Market Basket Analysis**  
- Learn how to implement **Apriori** and **FPGrowth** from scratch  
- Deep dive into **association rule metrics**: support, confidence, and lift  
- Master **data preprocessing**, **feature engineering**, and **one-hot encoding**  
- Get hands-on experience with **real retail datasets**  
- Compare algorithm performance for **scalability** and **efficiency**

---

## Hands-On Solution Code

[Market Basket Analysis Project
](https://www.projectpro.io/project-use-case/market-basket-analysis-apriori-fpgrowth)


## Key Concepts Covered

- **Market Basket Analysis (MBA)** – Definition, advantages, and use cases
- **Association Rules** – How they’re generated and interpreted
- **Apriori vs. FPGrowth** – Algorithmic differences and when to use which
- **Types of MBA** – Descriptive, Predictive, and Differential

---

## Real-World Applications

- **Retail Strategy**: Optimize store layouts & product placement  
- **Marketing**: Personalized promotions based on past purchases  
- **E-commerce**: Recommendation systems & combo offers  
- **Customer Insights**: Understand buying patterns for segmentation

---

> *This project is ideal for data science enthusiasts aiming to gain practical experience with association rule learning and derive business insights from transactional data.*

---

