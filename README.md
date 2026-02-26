💳 Explainable Credit Risk Scoring with XGBoost, SHAP & Tableau

📌 Project Overview

This is an end-to-end credit risk scoring system that predicts the probability of a loan applicant defaulting — and more importantly, explains why. Built on over 150,000 loan records, the project bridges the gap between complex machine learning models and real business decision-making using SHAP explainability and an interactive Tableau dashboard.

🎯 Designed for loan underwriters who need to understand not just the risk score, but the top factors driving each individual decision.

🎯 Business Problem

Financial institutions face a core challenge:

"How do we decide who gets a loan — and can we justify that decision?"

Traditional credit scoring models (like simple scorecards) lack predictive power. Modern ML models are powerful but often act as "black boxes" — which creates legal, ethical, and trust issues with customers and regulators.

🎯 This project solves both problems:

High-accuracy predictions using XGBoost
Full transparency using SHAP values per applicant
Business-friendly visualization via Tableau


📂 Project Structure

Credit-Risk-Scoring/

credit.ipynb          Main Jupyter Notebook (EDA, modeling, SHAP analysis)
Final_Data/           Processed dataset folder
README.md             Project documentation

🔍 Project Workflow

1️⃣ Data Collection & Exploration
- Dataset: 150,000+ loan applicant records
- Features include income, debt ratio, credit history, number of dependents, past-due payments, etc.
- Exploratory Data Analysis (EDA) to understand distributions and correlations

2️⃣ Data Cleaning & Feature Engineering
- Handled missing values and outliers using Pandas
- Created derived features:
  `IncomePerPerson` — income normalized by number of dependents
  `NumberOfPastDue` — aggregated past-due payment counts
  Debt-to-income ratio buckets
- Encoded categorical variables and scaled numerical features

3️⃣ Model Building
- Trained an XGBoost Classifier for binary classification (default vs. no default)
- Applied class imbalance handling using scale_pos_weight
- Hyperparameter tuning for optimal performance
- Evaluated using AUC-ROC, Precision, Recall, and F1 Score

4️⃣ Model Explainability with SHAP
- Computed global SHAP values → Which features matter most overall?
- Computed local SHAP values → Why did this specific applicant get this score?
- Generated waterfall plots and force plots per applicant
- Exported SHAP values to CSV for use in Tableau

5️⃣ Tableau Dashboard
- Imported model output + SHAP values into Tableau Public
- Built interactive dashboard for loan underwriters
- Applicant-level drill-down with risk score + factor breakdown

📊 Key Results

Metric Score
AUC-ROC 0.86
Precision High (minimizing false approvals)
Top Feature NumberOfTimes90DaysLate
Dataset Size 150,000+ records
Explainability Per-applicant SHAP breakdown

🔑 Key Insights

📌 Past-due payment history was the single strongest predictor of default
💰 Debt-to-income ratio above 40% significantly elevated risk scores
👨‍👩‍👧 Dependents combined with low income created a high-risk profile
🔁 Applicants with 3+ late payments in the last 2 years had 4x higher default rate
✅ SHAP explanations revealed that the model was fair and not relying on proxies** for protected attributes

🛠️ Tech Stack

Category & Tools 

Language: Python 3.8+ 
Data Analysis: Pandas, NumPy 
Machine Learning: Scikit-learn, XGBoost 
Explainability: SHAP 
Visualization (Code): Matplotlib, Seaborn 
Visualization (Dashboard): Tableau Public 
Environment: Jupyter Notebook 

🚀 How to Run Locally

Skills Demonstrated

✅ Exploratory Data Analysis (EDA) on large datasets
✅ Feature Engineering & Data Preprocessing
✅ Machine Learning Model Building (XGBoost)
✅ Model Evaluation (AUC-ROC, Precision, Recall)
✅ AI Explainability (SHAP — global & local)
✅ Business Dashboard Design (Tableau)
✅ Translating ML output into business-friendly insights

💼 Real-World Relevance

This project demonstrates skills directly applicable to roles in:
Data Analyst— EDA, visualization, business storytelling
Business Analyst— translating data into decisions
Risk Analyst— credit risk and financial modeling
Data Scientist— ML modeling and explainability

⭐ If you found this project useful or interesting, please consider giving it a star!
