**Fraud Detection System 🕵️‍♀️💳**

**📌 Project Overview**
This project focuses on detecting fraudulent financial transactions using Machine Learning.
The dataset provided had 6.3M transactions and 10 columns, and due to compute limits, a stratified sample of 50k rows was used for model development and evaluation.

**The pipeline covers:**
Data Cleaning (missing values, outliers, multicollinearity)
Feature Engineering (scaling numeric, encoding categorical)
Model Training (Logistic Regression with class balancing)
Model Evaluation (confusion matrix, precision, recall, ROC-AUC, PR-AUC)
Insights (key risk factors for fraud & prevention strategies)

**📊 Dataset**

Rows: 6,362,620
Columns: 10 (transaction type, amount, balances, fraud flag, etc.)
Target Variable: isFraud (1 = Fraudulent, 0 = Legitimate)
Source: Provided CSV file

⚙️ Methodology

**Data Preprocessing**
Dropped identifiers (nameOrig, nameDest)
Scaled numeric features with StandardScaler
One-hot encoded categorical type

**Model**
Logistic Regression (class_weight="balanced")
Pipeline used for clean workflow

**Evaluation Metrics**
Accuracy
Precision, Recall, F1-score
Confusion Matrix
ROC-AUC & PR-AUC

📈 **Results**
Fraud detection achieved with strong recall (catching frauds) while maintaining reasonable precision.
**Key Indicators of Fraud:**
Transaction type = TRANSFER / CASH_OUT
Large transaction amounts
Mismatched origin/destination balances

🔐 **Actionable Business Plan**
Implement real-time fraud scoring
Trigger step-up authentication (OTP, device check) for high-risk transfers
Apply velocity checks & limits on large transactions
Monitor feature drift and retrain regularly
