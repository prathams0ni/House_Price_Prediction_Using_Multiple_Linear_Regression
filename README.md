# House Price Prediction Using Multiple Linear Regression

## 📌 Project Overview
This project implements **Multiple Linear Regression** to predict house prices based on numerical property and neighborhood characteristics. The goal is to understand how various factors influence property value and evaluate model performance using standard regression metrics.

---

## 🎯 Problem Statement
Given a dataset of residential properties with numerical features, the objective is to:
- Predict house prices accurately
- Identify the most influential factors affecting property value
- Evaluate model performance using regression metrics

---

## 📂 Dataset Details
- **File Name:** `Houses.xlsx` / `linear_regression_numeric.csv`
- **Target Variable:** `price` (in $1000s)

### Features:
- `area_sqft` – Total built-up area
- `bedrooms` – Number of bedrooms
- `bathrooms` – Number of bathrooms
- `age_years` – Age of the house
- `distance_city_center_km` – Distance from city center
- `num_schools_nearby` – Schools within 3 km
- `crime_rate_index` – Crime severity index

---

## 🛠️ Tech Stack
- **Language:** Python
- **Libraries:**
  - pandas
  - numpy
  - matplotlib / seaborn
  - scikit-learn
- **Environment:** Jupyter Notebook

---

## 🔍 Methodology

### 1. Data Loading & Cleaning
- Imported numerical dataset
- Checked for missing values and data consistency

### 2. Exploratory Data Analysis
- Analyzed feature distributions
- Studied correlations between features and house price

### 3. Model Building
- Implemented **Multiple Linear Regression**
- Split data into training and testing sets
- Trained regression model on training data

### 4. Model Evaluation
- **R² Score:** Measures variance explained by the model
- **MAE:** Average absolute prediction error
- **RMSE:** Penalizes larger prediction errors

### 5. Model Interpretation
- Analyzed regression coefficients
- Identified positive and negative price drivers

---

## 📊 Key Results & Insights
- Model explains ~95% of price variance
- Area, bedrooms, bathrooms strongly increase price
- Distance from city center and crime rate reduce price
- Model shows strong generalization on test data

---

## 📈 Final Conclusion
The Multiple Linear Regression model provides accurate and interpretable house price predictions. It highlights key real-estate drivers and serves as a solid foundation for predictive analytics in property valuation.

---

## 🚀 How to Run
1. Clone the repository
2. Open the notebook in Jupyter
3. Install required libraries
4. Run all cells sequentially

---
