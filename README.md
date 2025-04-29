# 🛡️ Online Payment Fraud Detection - ML Project

This repository contains an end-to-end project for detecting fraudulent online payment transactions using Machine Learning.  
It includes data preprocessing, exploratory data analysis (EDA), model building with Logistic Regression.

---

## 📂 Project Structure

- **1. EDA.ipynb**  
  Performs exploratory data analysis to understand key patterns, trends, and relationships in the transaction data.

- **2. Fraud_Detection.ipynb**  
  - Preprocesses the data, handles class imbalance, and builds a Logistic Regression model on the balanced dataset.
  - Analyzes model performance using metrics like Precision, Confusion Matrix, and AUC-ROC curve.

---

## 📊 Dataset Description
https://www.kaggle.com/datasets/rupakroy/online-payments-fraud-detection-dataset

The dataset consists of online payment transactions with the following features:
- `step`: Time step in hours.
- `type`: Type of transaction (e.g., CASH_OUT, TRANSFER).
- `amount`: Transaction amount.
- `nameOrig`: Originating customer.
- `oldbalanceOrg`: Customer's balance before transaction.
- `newbalanceOrig`: Customer's balance after transaction.
- `nameDest`: Recipient customer.
- `oldbalanceDest`: Recipient's balance before transaction.
- `newbalanceDest`: Recipient's balance after transaction.
- `isFraud`: Target variable (1 = Fraudulent, 0 = Legitimate).

> Note:  
> - The original dataset has 6362620 transactions and was highly imbalanced (6354407 legitimate vs 8213 fraudulent transactions).  
> - A balanced temporary dataset (8213 legit and 8213 fraud transactions) was created for training the Logistic Regression model.  

---

## ⚙️ Technologies Used

- Python (Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn)

---

## 📈 Key Highlights

- **Achieved ~90% accuracy score** on both training and testing datasets using Logistic Regression on balanced data.
- **Evaluation Metrics**:
  - Precision Score
  - Confusion Matrix
  - AUC-ROC Curve and Score
- **Handled class imbalance** thoughtfully to design a reliable detection system.

---
## 🔍 Exploratory Data Analysis (EDA) Insights

- **Fraud Rate & Transaction Types**
  - Only 0.1% (8,213 out of 6.3M) transactions were fraudulent.
  - 100% of fraud cases occurred in just two transaction types: TRANSFER and CASH_OUT.
- **Temporal Trends**
  - Fraud peaked on Day 16 and dipped lowest on Day 23 (over 31 days).
- **Transaction Amounts**
  - Most fraudulent transactions fell within 100K–1.5M, suggesting targeted high-value fraud.
- **Class Imbalance**
  - **Extreme skew:** 99.9% legitimate vs. 0.1% fraudulent transactions, necessitating random under-sampling for modeling.

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/online-fraud-detection.git
