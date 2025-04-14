# FEAST Feature Store Example for Scaling Machine Learning

## Overview

This project demonstrates how to use **Feast (Feature Store)** to manage, store, retrieve, and serve features for machine learning models—specifically applied to a **customer churn prediction** problem. It walks through the entire workflow of integrating Feast into your ML pipeline for both **offline training** and **real-time inference**, solving common MLOps challenges like data consistency and feature reusability.

By the end of this project, you'll have built an end-to-end pipeline that:
- Retrieves training and serving features via Feast
- Trains machine learning models (Random Forest and Gradient Boosting)
- Performs real-time predictions through an API
- Showcases the architecture and command-line usage of Feast

---

## Business Objective

In customer-centric businesses, **churn prediction** is critical for proactive retention strategies. However, productionizing such models at scale is often hindered by inconsistent and scattered feature pipelines.

This project leverages **Feast**, an open-source feature store, to:
- Maintain feature consistency between training and serving
- Enable low-latency online inference
- Promote feature sharing and reuse across models

Through this example, you’ll gain hands-on experience using a feature store to scale ML operations and ensure reliability in production.

---

## Dataset

- **Source**: Simulated customer churn dataset
- **Total Records**: 891 customers
- **Features**:
  - `created_at` – Timestamp of data creation
  - `customer_id` – Unique identifier
  - `churned` – Target variable (1 if churned, 0 otherwise)
  - `category` – Customer category
  - `sex` – Gender
  - `age` – Age of the customer
  - `order_gmv` – Gross merchandise value of orders
  - `credit_type` – Type of credit plan

The dataset is used to demonstrate **entity definition**, **feature views**, and **training/serving flows** with Feast.

---

## Tech Stack

### Language
- **Python 3.x**

### Libraries & Tools
- **[Feast](https://docs.feast.dev/)** – Feature store for ML
- **Pandas** – Data manipulation
- **Scikit-learn** – ML model training (Random Forest, Gradient Boosting)
- **Flask** – Serving real-time inference API
- **Pickle** – Model serialization

---

## Project Workflow

### 1.Environment Setup
- Install Feast and dependencies
- Initialize and configure the Feast repository

### 2.Feature Store Configuration
- Define **Entities** (e.g., `customer_id`)
- Define **Feature Views** with associated data sources
- Set up **Offline Store** (for batch training) and **Online Store** (for real-time inference)

### 3.Feature Retrieval
- Use Feast CLI and SDK to retrieve historical features for training
- Validate feature pipelines and point-in-time correctness

### 4.Model Training
- Train models using retrieved features:
  - **Random Forest Classifier**
  - **Gradient Boosting Classifier**
- Save trained models as serialized `.pkl` files

### 5.Real-Time Inference
- Deploy a Flask API for real-time predictions
- Query the online store for fresh features using Feast SDK
- Serve predictions via REST endpoints (tested using Postman)

---

## Expected Outcomes

- A fully functional **Feature Store pipeline** for ML lifecycle management
- Offline → Online feature sync with point-in-time accuracy
- Trained churn prediction models ready for real-time inference
- Working API endpoint for serving churn predictions
- Clear understanding of how to use Feast in a production context

---

## Learning Takeaways

From this project, you will learn to:

- Understand and deploy the **Feast architecture** for real-world use cases
- Define **entities** and **feature views**
- Retrieve **offline** and **online features**
- Ensure **training-serving consistency**
- Integrate Feast into a real-time **model inference pipeline**
- Serve predictions via **Flask + Postman**

---

## Hands-On Solution Code
[FEAST Feature Store Project
](https://www.projectpro.io/project-use-case/feast-feature-store-example-for-scaling-machine-learning)
