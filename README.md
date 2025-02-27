# 🛒 ShopSmart Purchase Prediction Challenge

## 📌 Project Overview
This repository contains our submission for the **ShopSmart Purchase Prediction Challenge**, part of the **Foundations of Machine Learning** course at CentraleSupélec.  
Our goal is to build a predictive model to determine whether a customer will make a purchase based on behavioral data.  

- **Course**: DSBA - Foundations of Machine Learning  
- **Instructor**: Fragkiskos Malliaros  
- **Team Name**: YYDS  
- **Team Members**: Lanxin LI, Meng XIA, Hanqi YANG  

## 📊 Competition Description
ShopSmart, a leading e-commerce platform, wants to improve conversion rates by predicting which users are likely to make a purchase.  
Our task is to develop a machine learning model that analyzes user interactions and predicts purchasing behavior.  

- **Dataset**: Provided on Kaggle  
- **Task**: Multi-class classification  
- **Evaluation Metric**: Kaggle Leaderboard Score  

## 🚀 Pipeline Summary
Our approach follows a structured pipeline:

### **1️⃣ Exploratory Data Analysis (EDA)**
- **Checked for missing values** and imbalanced data.  
- **Data inconsistencies** (e.g., "afterno0n" vs. "afternoon") were handled.  
- **Class imbalance detected**, requiring resampling techniques (e.g., SMOTE).  

### **2️⃣ Feature Engineering**
- **Handled missing values**:
  - Numerical: Filled with mean values.  
  - Categorical: "unknown" category for high missing rates.  
- **One-hot encoding** for categorical variables.  
- **Feature scaling & normalization** for numerical data.  
- **Created new feature**:  
  - `Effective_Price = Price * (1 - Discount / 100)`

### **3️⃣ Model Selection & Tuning**
We tested various models and fine-tuned hyperparameters:  
✅ **XGBoost** (Best Performing)  
✅ **Logistic Regression** (with and without SMOTE)  
✅ **Random Forest**  

Our **final model** was selected based on **cross-validation performance** and **Kaggle leaderboard scores**.

## 📂 Repository Structure
```plaintext
📁 ShopSmart-Purchase-Prediction
│── 📄 README.md              # Project documentation  
│── 📄 report.pdf             # Kaggle Challenge Report  
│── 📂 data/                  # Training & evaluation datasets  
│── 📂 notebooks/             # Jupyter Notebooks for EDA & model training  
│── 📂 src/                   # Source code for preprocessing & modeling  
│── 📂 submissions/           # Kaggle submission files  
│── 📄 requirements.txt       # Dependencies  
