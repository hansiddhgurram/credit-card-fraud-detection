# 💳 Credit Card Fraud Detection

## 📌 Project Overview

This project builds a machine learning system to detect fraudulent credit card transactions.

The dataset is highly imbalanced, with fraudulent transactions representing only a small fraction of total transactions. The objective is to build a model that effectively identifies fraud while minimizing false negatives.

---

## 📊 Dataset

- Source: Public credit card transaction dataset
- Total transactions: ~284,000
- Fraudulent transactions: ~0.17%
- Features: 30 numerical features (including PCA-transformed variables V1–V28, Time, Amount)
- Target variable:
  - 0 → Normal transaction
  - 1 → Fraudulent transaction

---

## ⚠️ Key Challenge

The dataset is severely imbalanced.

Accuracy alone is misleading in fraud detection.  
This project focuses on:

- Recall (to catch fraudulent transactions)
- Precision (to reduce false alarms)
- F1-score
- ROC-AUC
- Precision-Recall curve

---

## 🧪 Project Workflow

### 1️⃣ Exploratory Data Analysis (EDA)
- Checked class imbalance
- Analyzed transaction amount distribution
- Compared fraud vs non-fraud behavior
- Correlation heatmap analysis

### 2️⃣ Preprocessing
- Scaled `Time` and `Amount`
- Stratified train-test split
- Applied SMOTE to balance training data

### 3️⃣ Modeling
Trained multiple models:
- Logistic Regression
- Random Forest

### 4️⃣ Advanced Evaluation
- ROC Curve & AUC
- Precision-Recall Curve
- Threshold tuning
- Comparison of recall vs precision trade-offs

---

## 📈 Results

- Successfully handled extreme class imbalance
- Achieved strong recall on fraudulent class
- Optimized threshold for better fraud detection performance

(You can optionally add actual metric values here after final testing.)

---

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Imbalanced-learn (SMOTE)
- Matplotlib
- Seaborn

---

## 📂 Project Structure
credit-card-fraud-detection/
│
├── notebooks/
│ ├── 1_eda.ipynb
│ ├── 2_preprocessing.ipynb
│ ├── 3_modeling.ipynb
│ └── 4_evaluation.ipynb
│
├── .gitignore
└── README.md