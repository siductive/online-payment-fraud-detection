# 🛡️ Online Payment Fraud Detection - ML Project

This repository contains an end-to-end project for detecting fraudulent online payment transactions using Machine Learning.  
It includes data preprocessing, exploratory data analysis (EDA), model building with Logistic Regression and Random Forest, and a Tableau dashboard for interactive data visualization.

---

## 📂 Project Structure

- **1. EDA.ipynb**  
  Performs exploratory data analysis to understand key patterns, trends, and relationships in the transaction data.

- **2. Fraud_Detection.ipynb**  
  - Preprocesses the data, handles class imbalance, and builds a Logistic Regression model on the balanced dataset.
  - Applies a Random Forest model to the original unbalanced dataset to better handle the natural class distribution.
  - Analyzes model performance using metrics like Precision, Confusion Matrix, and AUC-ROC curve.

- **3. Fraud_Detection_Dashboard.twb**  
  An interactive Tableau dashboard showcasing key metrics, transaction patterns, and fraud analysis.

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
> - The original dataset has 6362620 tarnsactions and was highly imbalanced (6354407 legitimate vs 8213 fraudulent transactions).  
> - A balanced temporary dataset (8213 legit and 8213 fraud transactions) was created for training the Logistic Regression model.  

---

## ⚙️ Technologies Used

- Python (Pandas, NumPy, Seaborn, Matplotlib, Scikit-learn)
- Tableau (for dashboarding and visualization)

---

## 📈 Key Highlights

- **Achieved ~90% accuracy score** on both training and testing datasets using Logistic Regression on balanced data.
- **Evaluation Metrics**:
  - Precision Score
  - Confusion Matrix
  - AUC-ROC Curve and Score
- **Handled class imbalance** thoughtfully to design a reliable detection system.
- **Developed an interactive Tableau dashboard** to visualize fraud patterns, transaction types, amount distributions, and time-based trends.

---

## 🚀 Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/online-fraud-detection.git
