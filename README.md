# 🚗 Car Price Prediction – Machine Learning Project

This project predicts car prices using machine learning regression models. The dataset is taken from a hypothetical Chinese automobile company entering the U.S. market. The goal is to identify key features influencing car prices and build a robust regression model.

---

## 📁 Dataset

- **File:** `CarPrice_Assignment.csv`
- **Source:** Provided as part of assignment
- **Target Variable:** `price`
- **Features:** Car specifications like engine size, horsepower, brand, etc.

---

## 🔧 Tasks Completed

### ✅ 1. Data Preprocessing
- Removed duplicates and irrelevant columns (`car_ID`)
- Extracted brand names from `CarName`
- Fixed misspelled brand names
- One-hot encoded categorical variables
- Scaled data for Support Vector Regressor

### ✅ 2. Model Implementation (5 Models)
Implemented and evaluated the following regression algorithms:
- Linear Regression
- Decision Tree Regressor
- Random Forest Regressor
- Gradient Boosting Regressor
- Support Vector Regressor (SVR)

### ✅ 3. Model Evaluation
Used:
- Mean Squared Error (MSE)
- R² Score

### ✅ 4. Feature Importance Analysis
- Identified top predictors of car price (e.g., `enginesize`, `curbweight`, `CarBrand_bmw`)
- Visualized using bar plots

### ✅ 5. Hyperparameter Tuning
- Performed `GridSearchCV` on Random Forest
- Improved R² from **0.9528 → 0.9554**
- Reduced MSE from **3.73M → 3.52M**

---

## 📊 Final Model Performance (Random Forest)

| Metric    | Original RF   | Tuned RF     |
|-----------|----------------|--------------|
| R² Score  | 0.9528         | **0.9554**   |
| MSE       | 3,725,492      | **3,520,776**|

---

## 📌 Requirements

```bash
pandas
numpy
scikit-learn
matplotlib
seaborn
