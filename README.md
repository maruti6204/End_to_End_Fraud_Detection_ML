# 📊 AI-Based Loan Default Prediction

An end-to-end Machine Learning project that predicts whether a borrower is likely to default on a loan using financial and behavioral features.

---

## 🚀 Project Overview

Loan default is a major challenge in banking and fintech. This project builds a predictive model using Machine Learning to identify high-risk borrowers before loan approval.

---

## 🎯 Objectives

- Build a binary classification model (Default / No Default)
- Maximize recall for defaulters
- Improve model accuracy
- Perform feature engineering
- Compare multiple ML models

---

## 💼 Business Impact

- Reduce bad loans (NPAs)
- Improve credit risk assessment
- Faster loan approvals
- Better financial decision-making

---

## 🧠 Feature Engineering

- **Loan_per_Month** → Monthly EMI burden  
- **Income_per_Month** → Monthly income  
- **Interest_Burden** → Loan cost pressure  
- **DTI_Loan** → Debt + loan risk  
- **Stress_Ratio** → EMI / Income (most important)  
- **Credit_DTI_Risk** → Credit weakness + debt  

---

## 📂 Dataset Features

- Income  
- Loan Amount  
- Interest Rate  
- Credit Score  
- Loan Term  
- Employment Type  
- Marital Status  
- Debt-to-Income Ratio  
- Default (Target)  

---

## 🔍 Key Insights

- Lower credit score → higher default risk  
- Higher DTI → higher risk  
- Financial stress strongly predicts default  
- Dataset is imbalanced  

---

## ⚙️ Methodology

1. Data Cleaning  
2. Feature Engineering  
3. Train-Test Split  
4. SMOTE (handle imbalance)  
5. Model Training  
6. Hyperparameter Tuning  
7. Cross Validation  
8. Evaluation  

---

## 🤖 Models Used

- Logistic Regression  
- XGBoost  

---

## 📈 Results

| Model                | Accuracy | Recall | ROC-AUC |
|---------------------|----------|--------|--------|
| Logistic Regression | ~68%     | ~69%   | ~0.85  |
| XGBoost             | ~83%     | ~76%   | ~0.88  |

---

## 💰 Business Cost Formula
Total Cost = (FN × Cost_FN) + (FP × Cost_FP)

- False Negative = ₹10,000 (high loss)  
- False Positive = ₹2,000  

---

## 📊 Evaluation Metrics

- Accuracy  
- Precision  
- Recall (Most Important)  
- F1 Score  
- ROC-AUC  
- Confusion Matrix  

---

## 🔍 Important Features

- Stress_Ratio  
- DTI-based features  
- Credit Score  
- Income  
- Loan Term  

---

## 🏗️ Deployment

- Streamlit Web App  
- Flask API  
- Cloud (AWS / Azure)  

---

## ⚖️ Ethics

- Avoid bias  
- Ensure transparency  
- Protect data privacy  
- Human oversight required  

---

## 🚧 Limitations

- No real-time data  
- Limited features  
- Imbalanced dataset  

---

## 🔮 Future Work

- Real-time prediction system  
- Integration with banking systems  
- Advanced models (LightGBM, Neural Networks)  

---

## 🛠️ Tech Stack

- Python  
- Pandas, NumPy  
- Scikit-learn  
- XGBoost  

---

## 👤 Author

**Maruti Nandan**  
MBA (AI & Data Science)  

---

⭐ If you like this project, give it a star!
