
# Explainable Credit Risk Scoring with XGBoost, SHAP, and Tableau

![Python](https://img.shields.io/badge/Python-3.8%2B-blue.svg)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)
![Libraries](https://img.shields.io/badge/Libraries-Pandas%20%7C%20XGBoost%20%7C%20SHAP-green.svg)
![Tool](https://img.shields.io/badge/Tool-Tableau-red.svg)

This repository contains the code and resources for an end-to-end data science project focused on building an explainable credit risk model. The project leverages a powerful XGBoost classifier and visualizes its predictions and their underlying drivers through an interactive Tableau dashboard, powered by SHAP values.

The primary goal is to create a tool that not only predicts the probability of a loan applicant defaulting but also provides clear, human-interpretable reasons for each decision, bridging the gap between complex models and business users.

## Final Product: Interactive Tableau Dashboard

The final output is an interactive dashboard designed for a loan underwriter. It allows them to select any applicant and instantly see their predicted risk score, the applicant's key financial details, and a breakdown of the top factors that increased or decreased their risk score.

*Click on an applicant on the left to see their risk drivers update on the right.*
Link : https://public.tableau.com/app/profile/gurnoor.singh7075/viz/CreditRisk_17520593887090/Dashboard1?publish=yes
![Tableau Dashboard Preview]

![image](https://github.com/user-attachments/assets/69f21a59-3f4c-4356-872f-f020ea3c0f1e)


## Project Highlights

-   **Advanced Modeling**: Engineered an XGBoost classifier on over 150,000 loan records.
-   **Model Explainability**: Computed and leveraged SHAP (SHapley Additive exPlanations) values to uncover both global feature importance and local, per-applicant prediction logic.
-   **Feature Engineering**: Processed and cleaned raw applicant data using Pandas, creating new derived metrics (e.g., `IncomePerPerson`, `NumberOfPastDue`) to enhance the model's predictive power.
-   **Interactive Visualization**: Designed and built a user-friendly Tableau dashboard that empowers non-technical users to explore and trust the model's outputs.

## Tech Stack

-   **Data Analysis & Modeling**: Python, Pandas, NumPy, Scikit-learn, XGBoost
-   **Model Explainability**: SHAP
-   **Data Visualization**: Matplotlib, Seaborn, Tableau Public
-   **Development Environment**: Jupyter Notebook
