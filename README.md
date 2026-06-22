# Credit Card Fraud Detection using Machine Learning

## Overview

This project focuses on detecting fraudulent credit card transactions using Machine Learning techniques. The dataset contains real-world credit card transactions and is highly imbalanced, with fraudulent transactions representing only a small fraction of the total data.

The objective is to build and evaluate classification models capable of accurately identifying fraudulent transactions while minimizing false alarms.

---

## Problem Statement

Financial institutions process millions of transactions daily, making manual fraud detection impractical. Machine Learning can help automate fraud detection by learning patterns from historical transaction data and identifying suspicious activities in real time.

---

## Dataset Information

- Total Transactions: **284,807**
- Fraudulent Transactions: **492**
- Fraud Percentage: **0.17%**
- Missing Values: **0**

The dataset is highly imbalanced, making accuracy alone an unreliable performance metric.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn

---

## Project Workflow

### 1. Data Exploration
- Loaded and inspected the dataset
- Examined dataset dimensions and data types

### 2. Data Quality Assessment
- Checked for missing values
- Verified data consistency

### 3. Exploratory Data Analysis (EDA)
- Analyzed fraud vs normal transaction distribution
- Calculated fraud percentage
- Investigated transaction amount patterns
- Visualized class imbalance

### 4. Data Preparation
- Defined feature and target variables
- Performed train-test split using stratified sampling

### 5. Model Development

#### Logistic Regression
Used as a baseline classification model with balanced class weights.

#### Random Forest Classifier
Implemented to improve fraud detection performance and handle complex feature relationships.

### 6. Model Evaluation
- Classification Report
- Confusion Matrix
- Precision
- Recall
- F1-Score

### 7. Feature Importance Analysis
Identified the most influential features contributing to fraud detection.

---

## Model Performance

### Logistic Regression

| Metric | Score |
|----------|----------|
| Precision | 0.05 |
| Recall | 0.92 |
| F1-Score | 0.10 |

### Random Forest

| Metric | Score |
|----------|----------|
| Precision | 0.96 |
| Recall | 0.74 |
| F1-Score | 0.84 |

---

## Confusion Matrix (Random Forest)

| | Predicted Normal | Predicted Fraud |
|----------|----------:|----------:|
| Actual Normal | 56,861 | 3 |
| Actual Fraud | 25 | 73 |

### Interpretation

- Correctly detected **73 fraudulent transactions**
- Missed **25 fraudulent transactions**
- Incorrectly flagged only **3 normal transactions as fraud**
- Achieved high precision with minimal false positives

---

## Top Important Features

The Random Forest model identified the following features as the most influential:

1. V14
2. V10
3. V12
4. V4
5. V17
6. V3
7. V11
8. V16
9. V2
10. V9

---

## Key Findings

- The dataset was highly imbalanced.
- No missing values were present.
- Logistic Regression achieved high recall but generated many false positives.
- Random Forest significantly improved precision and overall model performance.
- Feature importance analysis highlighted the variables most relevant for fraud detection.

---

## Conclusion

This project successfully developed a machine learning-based fraud detection system using credit card transaction data.

Among the evaluated models, **Random Forest** delivered the best performance with:

- Precision: **96%**
- Recall: **74%**
- F1-Score: **84%**

The model effectively identified fraudulent transactions while maintaining a very low false positive rate, making it a strong candidate for real-world fraud detection applications.

---

## Author

**Vidhi Mittal**

B.Tech Computer Science Engineering  
Meerut Institute of Engineering and Technology (MIET)
