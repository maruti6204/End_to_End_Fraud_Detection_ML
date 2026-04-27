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
⚙️ Methodology
Data Cleaning
Feature Engineering
Train-Test Split
Handling Imbalance (SMOTE)
Model Training
Hyperparameter Tuning
Cross Validation
Threshold Optimization
🤖 Models Used
🔹 Logistic Regression
Baseline interpretable model
🔹 XGBoost Classifier
High-performance boosting model
Captures complex relationships
📈 Model Performance
Model	Accuracy	Recall (Default)	ROC-AUC
Logistic Regression	~68%	~69%	~0.85
XGBoost	~83%	~76%	~0.88
✅ XGBoost outperformed Logistic Regression significantly
💰 Business Cost Analysis
In loan prediction:
❌ False Negative → High loss (bad loan approved)
⚠️ False Positive → Opportunity loss
Cost assumption:
FN = ₹10,000
FP = ₹2,000
Formula:
Total Cost = (FN × Cost_FN) + (FP × Cost_FP)
➡️ Model optimized to reduce False Negatives
📊 Evaluation Metrics
Accuracy
Precision
Recall ⭐ (Most Important)
F1 Score
ROC-AUC Curve
Confusion Matrix
The confusion matrix (shown in appendix pages) highlights:
Correct predictions
Missed defaults
False alarms
🔍 Model Interpretability
Top important features:
Stress_Ratio
DTI-based features
Credit Score
Income features
Loan Term
Feature importance from XGBoost shows engineered features dominate — which is ideal.
🏗️ Deployment
Possible deployment options:
🌐 Streamlit Web App
🔌 Flask API
☁️ Cloud (AWS / Azure)
⚖️ Ethical Considerations
Avoid bias (gender, caste, etc.)
Ensure transparency
Protect user data
Maintain human oversight
🚧 Limitations
Uses historical data only
No real-time integration
Limited dataset features
Class imbalance challenges
🔮 Future Improvements
Real-time loan scoring
Integration with banking systems
Use advanced models (LightGBM, Neural Networks)
Add more behavioral & demographic features
🛠️ Tech Stack
Python
Pandas, NumPy
Scikit-learn
XGBoost
Matplotlib / Seaborn
📌 Conclusion
This project demonstrates how Machine Learning can significantly improve credit risk prediction. Feature engineering combined with XGBoost delivers strong performance and real-world business value.
👤 Author
Maruti Nandan
MBA (AI & Data Science)
Graphic Era University
