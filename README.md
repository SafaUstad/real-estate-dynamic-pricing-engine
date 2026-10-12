# Real Estate Dynamic Pricing Engine

A machine learning pipeline designed to predict residential property values accurately using real-world real estate data, advanced feature engineering, and robust ensemble modeling.

## 🚀 Project Overview
Developed a dynamic valuation engine to estimate property prices based on features such as square footage, number of bedrooms, property age, geographic location, and income demographics[cite: 1]. The engine integrates data preprocessing, outlier removal, and non-linear regression to optimize prediction accuracy.

## 🛠️ Tech Stack
* **Language:** Python[cite: 1]
* **Data Manipulation & Cleaning:** Pandas, NumPy[cite: 1]
* **Machine Learning:** Scikit-learn, Random Forest Regressor[cite: 1]
* **Visualization:** Matplotlib, Seaborn

## 📊 Workflow Architecture
1. **Data Ingestion & Inspection:** Loading raw housing data and inspecting structural columns and data types.
2. **Feature Engineering:** Creating domain-specific ratios (e.g., *rooms per household*, *bedrooms per room*, *population density*) to capture hidden valuation signals.
3. **Outlier Removal:** Applying the Interquartile Range (IQR) method to eliminate extreme anomalies.
4. **Data Splitting:** Executing a strict **60-20-20 split** (60% Training, 20% Validation, 20% Test) to prevent data leakage and ensure robust generalization.
5. **Preprocessing Pipelines:** Handling missing values via median imputation and standardizing numerical features using `StandardScaler` and `OneHotEncoder`.
6. **Model Training & Evaluation:** Training a Random Forest Regressor and evaluating performance using **R² Score** and **RMSE**.

## 📈 Model Performance
* **Validation R² Score:** 0.7112
* **Validation RMSE:** $57,799.02
* **Test R² Score:** 0.6926
* **Test RMSE:** 0.6926

## 📂 Repository Structure
```text
real-estate-dynamic-pricing-engine/
│
├── notebooks/
│   └── Real_Estate_Dynamic_Pricing_Engine.ipynb
├── assets/
│   └── valuation_charts.png
└── README.md
