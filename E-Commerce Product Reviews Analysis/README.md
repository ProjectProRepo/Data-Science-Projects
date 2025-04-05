# E-commerce Product Reviews – Pairwise Ranking and Sentiment Analysis

This project applies machine learning techniques to analyze e-commerce product reviews. It focuses on performing **sentiment analysis** and developing a **pairwise ranking model** to prioritize reviews based on their relevance. This enhances the user experience by surfacing the most useful reviews at the top.

---

## Overview

Online product reviews can significantly influence purchasing decisions. However, the vast number of reviews often overwhelms users, making it hard to find meaningful feedback. This project solves that problem by:

- Detecting and filtering low-quality reviews (e.g., gibberish, profanity)
- Performing **sentiment analysis** to understand the tone and subjectivity
- Extracting features that capture the **relevance** of each review
- Using **Pairwise Learning to Rank (LTR)** to reorder reviews based on usefulness
- Converting the ranking problem into a classification task for model training

Through this approach, the project simulates how intelligent review filtering can enhance product discovery and customer satisfaction.

---

## Dataset

- **Source**: E-commerce platform (Simulated/Anonymized dataset)
- **Contents**: Text reviews, product IDs, user IDs, ratings
- **Attributes**:
  - `review_text`: Raw review content
  - `rating`: Numerical product rating (1–5)
  - `product_id`: Product identifier
  - `review_id`: Unique review identifier
  - `label_relevance`: Binary target indicating relevance for pairwise ranking

---

## Tech Stack

- **Languages**: Python
- **Libraries**:
  - `pandas`, `numpy` – Data manipulation
  - `matplotlib`, `seaborn` – Data visualization
  - `nltk`, `textblob`, `spacy` – NLP and text analysis
  - `scikit-learn` – ML models and evaluation
  - `langdetect`, `profanity-check`, `pyspellchecker` – Text preprocessing
  - `joblib` – Model serialization

---

## Project Workflow

### 1.Problem Understanding & Literature Review
- Study review relevance, sentiment analysis, and Learning-to-Rank methods.

### 2.Exploratory Data Analysis (EDA)
- Analyze review length, sentiment distributions, rating patterns.
- Explore language quality and potential bias.

### 3.Text Preprocessing
- **Language Detection**: Filter non-English reviews
- **Gibberish Detection**: Use Markov Chains to detect incoherent text
- **Profanity Detection**: Remove inappropriate content
- **Spelling Correction**: Fix misspelled words to improve model performance

### 4.Feature Engineering
- Extract:
  - **Sentiment Polarity** and **Subjectivity** (TextBlob)
  - **TF-IDF Vectors** for richness
  - **Readability Scores**
  - **Review Length**, **Punctuation Usage**, and other handcrafted features

### 5. Learning to Rank
- Understand Pointwise vs Pairwise vs Listwise LTR
- Choose **Pairwise Ranking** for this problem

### 6.Pairwise Review Generation
- Create review pairs per product
- Assign binary relevance labels to identify which review is more useful

### 7. Convert Ranking → Classification
- Treat each pair as a binary classification problem
- Train classification models to predict the more relevant review in a pair

### 8.Model Training & Evaluation
- **Model**: Random Forest Classifier (spot-checked with other classifiers)
- **Metrics**:
  - Classification Accuracy
  - Pairwise Ranking Accuracy (how well review order is preserved)
- Perform hyperparameter tuning and cross-validation

### 9. Model Saving & Pipeline Setup
- Save the trained model using `joblib`
- Build a data-to-prediction pipeline for future integration into apps

---

## Expected Outcomes

- Cleaned and structured dataset of high-quality, relevant product reviews
- A trained classifier capable of pairwise ranking
- Reordered reviews based on their estimated usefulness
- A modular codebase that can be extended to other NLP ranking tasks

---

## Learning Takeaways

- Best practices in **text data preprocessing** for real-world review datasets
- Techniques for **detecting gibberish and profanity** using probabilistic and rule-based approaches
- Use of **sentiment analysis**, **TF-IDF**, and custom NLP features
- Implementation of **Pairwise Learning to Rank** via classification
- Evaluation of ranking systems using both traditional and rank-specific metrics
- Construction of an **end-to-end machine learning pipeline**

---

## Hands-On Solution Code

[Ecommerce product reviews - Pairwise ranking and sentiment analysis
](https://www.projectpro.io/project-use-case/ecommerce-product-reviews-ranking-sentiment-analysis)
