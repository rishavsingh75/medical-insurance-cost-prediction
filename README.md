# 🏥 Medical Insurance Cost Prediction

A machine learning project that predicts insurance charges based on demographic, health, and lifestyle features using multiple regression models.

---

## 📌 Problem Statement

Insurance companies need accurate prediction of medical costs to optimize premium pricing and manage financial risk.  
The objective of this project is to build and compare multiple regression models to predict insurance charges using customer health and lifestyle data.

---

## 🎯 Project Objective

- Perform Exploratory Data Analysis (EDA)
- Identify key drivers of insurance charges
- Train multiple regression models
- Compare performance using R², MAE, and RMSE
- Select the best-performing model
- Provide business insights for pricing strategy

---

## 🧠 Dataset Features

The dataset includes:

- age
- bmi
- children
- gender
- smoker
- region
- annual_income
- policy_type
- pre_existing_disease
- hospital_visits_last_year
- exercise_hours_per_week
- alcohol_consumption_per_week
- cholesterol_level
- blood_pressure
- insurance_charges (Target Variable)

---

## 📊 Exploratory Data Analysis

Key observations:

- Insurance charges are positively skewed (presence of high-cost outliers).
- Smoking status shows strong impact on insurance charges.
- BMI and hospital visits have moderate correlation with cost.
- Individual numeric features show weak linear correlation, suggesting non-linear relationships.

---

## 🤖 Models Used

The following regression models were implemented:

- Linear Regression
- Ridge Regression
- Lasso Regression
- ElasticNet
- Random Forest Regressor
- Gradient Boosting Regressor

---

## 📈 Model Performance

| Model            | R² Score | MAE  | RMSE |
|------------------|----------|------|------|
| Gradient Boost   | 0.8795   | 1693 | 2148 |
| Random Forest    | 0.8723   | 1743 | 2212 |
| ElasticNet       | 0.8179   | 1863 | 2642 |
| Lasso            | 0.8178   | 1864 | 2642 |
| Ridge            | 0.8178   | 1864 | 2642 |
| Linear Regression| 0.8178   | 1864 | 2643 |

---

## 🏆 Final Model Selection

Gradient Boosting achieved the highest R² score (0.879) and the lowest error metrics.  
This indicates strong predictive performance and better generalization compared to linear models.

---

## 📌 Why Tree-Based Models Performed Better

- Target variable is skewed.
- Weak linear correlation between features and target.
- Non-linear relationships exist between health factors and insurance cost.
- Ensemble models capture feature interactions more effectively.

---

## 💼 Business Insights & Recommendations

1. Smoking status significantly increases insurance charges.
2. Higher BMI and frequent hospital visits contribute to increased costs.
3. Predictive modeling enables risk-based premium pricing.
4. Insurance companies can use this model to improve underwriting accuracy.
5. Preventive health programs targeting high-risk individuals may reduce long-term claims.

---

## 🛠 Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- gradio(for interface prototype)
- statsmodel
- scipy

---

## 📂 Project Structure

medical_insurance_cost.ipynb  
README.md  

---

## 👨‍💻 Author

Rishav Kumar Singh 
Data Analytics & Machine Learning Enthusiast
