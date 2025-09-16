# Wine Quality Analysis - Day 1 Assignment

**Intern:** Siddhartha Shakya 
**Company:** Amnil Technology  
**Date:** September 15, 2025

## Project Overview

This project implements machine learning models to analyze and predict wine quality using the Portuguese "Vinho Verde" wine dataset. The analysis includes both logistic regression for binary classification and linear regression for continuous quality prediction.

## Dataset Information

- **Source:** UCI Machine Learning Repository - Wine Quality Dataset
- **Types:** Red and white wine variants
- **Samples:** ~6,497 wine samples total
- **Features:** 11 physicochemical properties
- **Target:** Wine quality scores (3-9)

## Features Analyzed

1. Fixed acidity
2. Volatile acidity
3. Citric acid
4. Residual sugar
5. Chlorides
6. Free sulfur dioxide
7. Total sulfur dioxide
8. Density
9. pH
10. Sulphates
11. Alcohol

## Analysis Components

### Exploratory Data Analysis (EDA)
- Dataset overview and statistics
- Quality distribution analysis
- Feature distribution visualization
- Correlation analysis
- Outlier detection

### Data Preprocessing
- Feature scaling and normalization
- Binary encoding for wine type
- Train-test data splitting
- Feature importance analysis

### Machine Learning Models

#### 1. Logistic Regression
- **Purpose:** Binary classification (High/Low quality)
- **Target:** Quality ≥ 7 = High quality, < 7 = Low quality
- **Metrics:** Accuracy, Precision, Recall, F1-Score, ROC-AUC

#### 2. Linear Regression
- **Purpose:** Continuous quality score prediction
- **Target:** Exact quality scores (3-9)
- **Metrics:** R², RMSE, MAE, MSE

### Model Comparison
- Side-by-side performance analysis
- Feature coefficient comparison
- Prediction distribution analysis
- Recommendations for model selection

## Key Findings

- **Most Important Features:** Alcohol content, volatile acidity, and sulphates have the strongest impact on wine quality
- **Model Performance:** Both models show good predictive capability with different use cases
- **Data Insights:** Most wines are average quality (5-6), with few excellent (8-9) or poor (3-4) wines

## Technologies Used

- **Python 3.x**
- **Libraries:**
  - pandas - Data manipulation
  - numpy - Numerical computations
  - matplotlib & seaborn - Data visualization
  - scikit-learn - Machine learning models and preprocessing

## Files Structure

```
├── wine_quality_analysis.ipynb    # Main analysis notebook
├── datasets/
│   └── wines/
│       ├── winequality-red.csv    # Red wine dataset
│       ├── winequality-white.csv  # White wine dataset
│       └── winequality.names      # Dataset description
└── README.md                      # Project documentation
```

## How to Run

1. Clone this repository
2. Install required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn jupyter
   ```
3. Open `wine_quality_analysis.ipynb` in Jupyter Notebook or VS Code
4. Run all cells to reproduce the analysis

## Results Summary

- **Logistic Regression Accuracy:** ~[accuracy_value]
- **Linear Regression R² Score:** ~[r2_value]
- **Key Insight:** Alcohol content is the strongest positive predictor of wine quality
- **Business Application:** Models can help wineries optimize production for quality improvement

## Future Improvements

- Feature engineering for better predictive power
- Advanced models (Random Forest, Gradient Boosting)
- Cross-validation for robust performance estimation
- Hyperparameter tuning for optimal results

---

*This project was completed as part of the internship program at Amnil Technology.*
