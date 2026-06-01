# House Price Prediction - Machine Learning Project

## 📋 Project Overview

This notebook contains a comprehensive machine learning analysis for **predicting house prices** using the Kansas City (KC) Housing Dataset. The project implements three different regression models and compares their performance.

**Dataset**: KC House Data with 21,613 records and 21 features

---

## 📊 Notebook Content Summary

### 1. **Data Loading & Exploration**
- Installs required libraries: `pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`
- Loads KC House dataset from CSV
- Displays first 5 rows and dataset information
- Checks for missing values (Result: **No missing values found**)

### 2. **Feature Selection**
The following **16 features** are used for prediction:
- `bedrooms`
- `bathrooms`
- `sqft_living`
- `sqft_lot`
- `floors`
- `waterfront`
- `view`
- `condition`
- `grade`
- `sqft_above`
- `sqft_basement`
- `yr_built`
- `yr_renovated`
- `zipcode`
- `lat` (latitude)
- `long` (longitude)

**Target Variable**: `price`

### 3. **Data Preprocessing**
- 80-20 Train-Test Split (random_state=42)
- Training samples: 17,290
- Testing samples: 4,323

### 4. **Machine Learning Models**

#### **Model 1: Linear Regression**
```
Results:
- MAE (Mean Absolute Error): $127,744.43
- MSE (Mean Squared Error): 45,362,119,293.29
- RMSE (Root Mean Squared Error): $212,983.85
- R² Score: 0.6999 (70%)
```

#### **Model 2: Decision Tree Regressor**
```
Results:
- R² Score: 0.7074 (70.74%)
```

#### **Model 3: Random Forest Regressor** ⭐ **BEST PERFORMANCE**
```
Results:
- R² Score: 0.8518 (85.18%)
```

### 5. **Visualizations**

#### Chart 1: Actual vs Predicted House Prices
- Scatter plot showing the relationship between actual and predicted prices
- Helps identify model accuracy and outliers

#### Chart 2: Correlation Heatmap
- Shows correlations between all numerical features
- Color-coded: Red (positive) and Blue (negative) correlations
- Useful for identifying feature relationships

---

## 🎯 Model Performance Comparison

| Model | R² Score | Accuracy |
|-------|----------|----------|
| Linear Regression | 0.6999 | 70% |
| Decision Tree | 0.7074 | 70.74% |
| Random Forest | **0.8518** | **85.18%** ✅ |

**Best Model**: Random Forest Regressor with **85.18% accuracy**

---

## 📈 Key Findings

1. **No Missing Data**: The dataset is clean with no null values
2. **Feature Correlations**: Strong correlations exist between certain features and price
3. **Model Comparison**: Ensemble methods (Random Forest) outperform single algorithms
4. **Prediction Accuracy**: Random Forest achieves ~85% variance explanation

---

## 🛠 Technologies Used

- **Language**: Python 3.12
- **Libraries**:
  - `pandas` (2.2.2) - Data manipulation
  - `numpy` (2.0.2) - Numerical operations
  - `scikit-learn` (1.6.1) - Machine learning
  - `matplotlib` (3.10.0) - Visualization
  - `seaborn` (0.13.2) - Statistical visualization

---

## 📝 How to Use

### Run in Google Colab (Recommended)
```
Open: https://colab.research.google.com
File → Open notebook → GitHub
Enter: h399491-jpg/skillbit-technology
Select: Copy_of_Welcome_To_Colab.ipynb
```

### Run Locally
```bash
# Install dependencies
pip install pandas numpy matplotlib seaborn scikit-learn

# Run Jupyter notebook
jupyter notebook Copy_of_Welcome_To_Colab.ipynb
```

---

## 📂 Dataset Details

**Total Records**: 21,613
**Total Features**: 21 (including ID and target)

### Feature Types:
- **Numerical**: 15 features (int64, float64)
- **Categorical/Date**: 1 feature (date as object)
- **ID**: 1 feature

### Sample Data:
```
First house record:
- Price: $221,900
- Bedrooms: 3
- Bathrooms: 1.00
- Square Feet Living: 1,180
- Year Built: 1955
```

---

## ✅ Results Summary

✓ Dataset cleaned and validated  
✓ Features engineered and selected  
✓ 3 models trained and evaluated  
✓ Random Forest achieved best performance (85.18%)  
✓ Visualizations created for analysis  

---

## 📧 Author

**GitHub**: h399491-jpg  
**Repository**: skillbit-technology

---

## 📄 License

This project is shared on GitHub for educational purposes.

---

## 🔗 Links

- [View Notebook on GitHub](https://github.com/h399491-jpg/skillbit-technology/blob/main/Copy_of_Welcome_To_Colab.ipynb)
- [Open in Google Colab](https://colab.research.google.com/github/h399491-jpg/skillbit-technology/blob/main/Copy_of_Welcome_To_Colab.ipynb)

---

**Last Updated**: June 2026
