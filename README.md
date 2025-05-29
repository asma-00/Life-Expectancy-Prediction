# Life-Expectancy-Prediction

This project aims to predict **Life Expectancy** based on various health, economic, and demographic indicators using machine learning regression models.

---

## Dataset

This project uses the Life Expectancy (WHO) dataset (https://www.kaggle.com/datasets/kumarajarshi/life-expectancy-who) available on Kaggle.
It contains socio-economic and health-related indicators for multiple countries over several years, aiming to predict life expectancy.

---

## Project Steps

1. **Data Cleaning & Preprocessing**
   - Missing value imputation
   - Duplicate and formatting cleanup
   - Categorical encoding (`status`)
   - Feature scaling using `StandardScaler`

2. **Exploratory Data Analysis**
   - KDE plots for distribution
   - Correlation heatmap
   - Boxplots and histograms
   - Class balance analysis

3. **Feature Selection**
   - Correlation analysis
   - VIF to remove multicollinearity
   - Feature importance via:
     - RandomForestRegressor
     - LinearRegression (SelectKBest)

4. **Modeling**
   - Linear Regression
   - Ridge Regression
   - Random Forest Regressor ✅
   - XGBoost Regressor

5. **Evaluation**
   - R² and RMSE
   - 5-Fold Cross-Validation
   - Residual analysis

---

## Best Performing Model

| Model               | R²       | RMSE     |
|--------------------|----------|----------|
| Random Forest       | 0.9676   | 2.80     |
| XGBoost             | 0.9646   | 3.06     |
| Ridge Regression    | 0.8155   | 15.96    |
| Linear Regression   | 0.8155   | 15.96    |

- **Final Model Saved**: Random Forest Regressor using `joblib`.

---

## Tech Stack

- Python (Pandas, NumPy, Matplotlib, Seaborn)
- Scikit-learn
- XGBoost
- Joblib

---

