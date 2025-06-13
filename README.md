# 🏡 Bengaluru House Price Prediction
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/tanusree03/House_Price_Prediction/blob/main/House_Price_Prediction.ipynb)



A machine learning regression project that predicts housing prices in Bengaluru based on features like location, BHK, total square feet, and number of bathrooms. The goal is to provide a reliable model that estimates property prices using real-world data.

## 📌 Overview

This project uses data preprocessing, feature engineering, outlier handling, and various regression models (including Random Forest with hyperparameter tuning) to predict property prices. It also includes evaluation using R² score, MAE, and RMSE, along with visualization of predicted vs. actual values.

## 📊 Dataset

- **Source**: [Bengaluru House Price Data – Kaggle](https://www.kaggle.com/datasets/amitabhajoy/bengaluru-house-price-data?resource=download)
- Contains features like `location`, `size`, `total_sqft`, `bath`, and `price`.

## 🧠 Technologies & Libraries

- Python 🐍
- Pandas, NumPy
- Scikit-learn (LinearRegression, RandomForest, GridSearchCV)
- Matplotlib / Seaborn for visualization
- Google Colab

## ⚙️ ML Workflow

1. Data Cleaning & Transformation
   - Handle missing values
   - Convert textual sqft ranges to numerical
   - Extract BHK from size column
2. Outlier Removal
   - Based on sqft per BHK and price per sqft
3. Encoding
   - One-hot encoding for location
4. Model Building
   - Random Forest Regressor
   - GridSearchCV for tuning
5. Evaluation
   - R² Score ≈ 0.59 on test set
   - MAE ≈ ₹35 Lakhs
   - RMSE ≈ ₹100 Lakhs

---

## 📈 Example Output

```python
Prediction: ₹78,45,000 for a 2BHK in Whitefield with 1200 sqft
