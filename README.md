# House Price Prediction - Linear Regression

This project demonstrates the implementation of **Linear Regression** to predict house prices based on various property features. The notebook contains two separate implementations using data from different file formats (Excel and CSV) to showcase data handling versatility.

## 📁 Project Structure:

- **File**: `Linear_Regression.ipynb`
- **Data Sources**:
  - `Houses.xlsx` - Excel format housing data
  - `linear_regression_numeric.csv` - CSV format housing data

## 🏠 Dataset Description:

The dataset contains 200 records with the following features:

| Feature | Description | Data Type |
|---------|-------------|-----------|
| `area_sqft` | Total area of the house in square feet | Integer |
| `bedrooms` | Number of bedrooms | Integer |
| `bathrooms` | Number of bathrooms | Integer |
| `age_years` | Age of the property in years | Integer |
| `distance_city_center_km` | Distance from city center in kilometers | Float |
| `num_schools_nearby` | Number of schools in the vicinity | Integer |
| `crime_rate_index` | Crime rate index of the area | Float |
| `price` | Target variable - House price | Float |

## 🛠️ Implementation Details:

### Data Preprocessing
- ✅ No missing values detected in either dataset
- ✅ Data types appropriately assigned
- ✅ Statistical analysis performed using `describe()`

### Model Training
- **Algorithm**: Linear Regression from `sklearn.linear_model`
- **Train-Test Split**: 80-20 split using `train_test_split`
- **Random State**: 42 for reproducible results

### Model Performance

Both implementations (Excel and CSV) achieved identical performance metrics:

| Metric | Value | Interpretation |
|--------|-------|----------------|
| **R² Score** | 0.9564 | Excellent fit (95.64% variance explained) |
| **MAE** | 21.90 | Mean Absolute Error in price units |
| **RMSE** | 25.84 | Root Mean Square Error in price units |

### Feature Coefficients

The linear regression model identified the following relationships:

| Feature | Coefficient | Impact on Price |
|---------|-------------|-----------------|
| `area_sqft` | +0.119 | Positive but small effect |
| `bedrooms` | +13.97 | Strong positive effect |
| `bathrooms` | +13.04 | Strong positive effect |
| `age_years` | -1.85 | Negative effect (depreciation) |
| `distance_city_center_km` | -8.18 | Strong negative effect |
| `num_schools_nearby` | +5.46 | Positive effect |
| `crime_rate_index` | -10.92 | Strong negative effect |

## 📊 Key Insights:

1. **Location Matters**: Distance from city center and crime rate have significant negative impacts on house prices
2. **Property Features**: Bedrooms and bathrooms contribute positively to property value
3. **Age Factor**: Older properties tend to have lower values
4. **Amenities**: Proximity to schools increases property value

## 🚀 How to Run:

1. Clone the repository
2. Ensure you have the required libraries:
   ```bash
   pip install pandas scikit-learn numpy

## Final Output:
<img width="931" height="512" alt="image" src="https://github.com/user-attachments/assets/e13c4ea5-6f45-4377-acc8-695aedb7d7b9" />
