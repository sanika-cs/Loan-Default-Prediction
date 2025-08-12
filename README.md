# Lending Loan Default Prediction using Ensemble Models

This project presents a supervised machine learning pipeline to predict the risk of loan default using tabular financial data. It leverages ensemble learning techniques and advanced tools for model tuning, interpretation, and deployment.

---
## Dataset

The dataset used for this project is sourced from Kaggle:  
[Kaggle Loan Default Dataset](https://www.kaggle.com/datasets/saurabh13nov/lending-club-loan-data)  

The dataset contains financial and personal information of loan applicants, with a significant class imbalance:  
- **80%** of applicants did **not** default  
- **20%** of applicants **defaulted** on their loans  

To address this imbalance, the ADASYN oversampling technique was applied during preprocessing to improve model performance and reduce bias toward the majority class.

## Key Features

- **Data Preprocessing:**  
  Extensive preprocessing including outlier detection, handling missing values, and feature engineering.

- **Class Imbalance Handling:**  
  Applied ADASYN (Adaptive Synthetic Sampling) to balance the dataset and improve model generalization.

- **Models Trained:**  
  - Logistic Regression  
  - Random Forest  
  - LightGBM  
  - XGBoost  
  - CatBoost

- **Hyperparameter Optimization:**  
  Utilized the Optuna framework to perform automated and efficient hyperparameter tuning for optimal performance.

- **Stacking Ensemble:**  
  Created a stacking classifier using Logistic Regression as the meta-model and LightGBM, XGBoost, and CatBoost as base learners to boost predictive power.

- **Model Interpretability:**  
  Applied SHAP (SHapley Additive exPlanations) to interpret model predictions and identify the key features influencing loan default risk.

- **Experiment Tracking:**  
  Used MLflow for tracking experiments, logging parameters, and managing model versions throughout the development lifecycle.

- **Deployment:**  
  Developed and deployed the final model as an interactive web application using Streamlit for real-time loan default risk prediction.

---
## Screenshots

### Web App -streamlit

![App Screenshot](Screenshot%202025-08-12%20203921.png)

