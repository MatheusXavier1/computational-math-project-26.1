# Predicting Purchase Probability in E-commerce
## COC351 — Computational Mathematics | UFRJ 2026.1

---

## Overview

This project applies numerical methods to predict the probability 
of purchase in an e-commerce environment, using the 
**Online Shoppers Purchasing Intention** dataset from UCI Machine Learning Repository.

The goal is to identify which user sessions are most likely to result 
in a purchase, enabling better prioritization of marketing and sales efforts.

---

## Problem Statement

Given user behavior data from an e-commerce website, estimate:
- The probability of a customer completing a purchase
- How different factors influence that probability
- The optimal decision threshold to maximize conversion rate

---

## Dataset

- **Source**: UCI Machine Learning Repository
- **Link**: https://archive.ics.uci.edu/ml/machine-learning-databases/00468/online_shoppers_intention.csv
- **Size**: 12,330 sessions × 18 features
- **Target**: Revenue (True/False)
- **Class distribution**: 84.5% no purchase, 15.5% purchase

---

## Methodology

### 1. Exploratory Data Analysis
- Missing values verification
- Outlier detection (IQR method)
- Feature distribution analysis
- Target imbalance assessment

### 2. Data Preprocessing
- One-hot encoding for categorical variables (Month, VisitorType)
- StandardScaler normalization for numerical features (Z-score)
- Train/test split (70/30)

### 3. Modeling — Topic 1: Regression
- Logistic Regression to predict purchase probability
- Model evaluation: Accuracy, Precision, Recall, F1-score

### 4. Optimization — Topic 2: Extrema Search
- ROC Curve analysis
- Threshold optimization to maximize conversion rate
- Numerical method: finding maximum of f(threshold)

---

## COC351 Topics Covered

| Topic | Application |
|-------|-------------|
| Interpolation and Regression | Logistic Regression model |
| Extrema Search | Threshold optimization via ROC |

---

## Requirements
pandas
numpy
scikit-learn
matplotlib
scipy

---

## Authors

- Charles
- Matheus

UFRJ — Escola Politécnica  
COC351 — Computational Mathematics — 2026.1  
Supervisor: Prof. Frederico C. Jandre de A. Tavares
