📊 AI-Based Loan Default Prediction
An end-to-end Machine Learning project that predicts whether a borrower is likely to default on a loan using financial and behavioral features. This system helps financial institutions improve risk assessment and reduce bad loans.
🚀 Project Overview
Loan default is a major challenge in banking and fintech. Traditional methods are often slow and inaccurate.
This project builds a predictive model using:
Logistic Regression (baseline)
XGBoost (advanced model)
The system analyzes borrower data and predicts default risk before loan approval.
🎯 Objectives
Build a binary classification model (Default / No Default)
Maximize recall for defaulters (critical in finance)
Improve overall accuracy
Perform feature engineering for better predictions
Compare multiple ML models
💼 Business Impact
📉 Reduce Non-Performing Assets (NPAs)
💰 Minimize financial losses
⚡ Faster loan approval decisions
🎯 Better risk-based pricing
📊 Improved credit scoring
🧠 Key Features (Feature Engineering)
One of the strongest parts of this project is advanced feature engineering:
1. Loan_per_Month
Monthly EMI burden
Helps measure repayment pressure
2. Income_per_Month
Converts annual income → monthly income
Aligns with EMI payments
3. Interest_Burden
Combines loan amount + interest rate
Captures cost of borrowing
4. DTI_Loan
Combines Debt-to-Income ratio + loan amount
Measures leveraged risk
5. Stress_Ratio ⭐ (Most Important)
Loan_per_Month / Income_per_Month
Directly captures financial stress
Stress Ratio	Risk Level
< 0.2	Low
0.2–0.4	Moderate
> 0.4	High
> 0.6	Very High 🚨
6. Credit_DTI_Risk
Combines credit score weakness + debt pressure
Uses benchmark score (700)
📂 Dataset
Features used:
Income
Loan Amount
Interest Rate
Credit Score
Loan Term
Employment Type
Marital Status
Debt-to-Income Ratio
Default (Target)
🔍 Exploratory Data Analysis (EDA)
Key insights:
Lower credit score → higher default risk
Higher DTI ratio → higher probability of default
Financial stress strongly correlates with default
Dataset shows class imbalance
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
