# Life Expectancy Prediction Project Report
### Objective:
To analyze and predict life expectancy using socio-economic and health-related features from a global dataset. The goal was to build a reliable regression model capable of estimating life expectancy and understanding key contributing factors.

## Steps and Workflow:
### 1. Data Cleaning & Preprocessing
- Checked for missing values and imputed them using appropriate strategies (mean, mode, or interpolation).
- Removed duplicate rows and corrected column formatting (e.g., double spacing).
- Detected and handled outliers.
- Dropped highly correlated or redundant features (infant_deaths, thinness_5-9_years).
- Converted categorical data:
- status was mapped to binary (Developing = 0, Developed = 1).
- Scaled the numerical features using StandardScaler.

### 2. Exploratory Data Analysis (EDA)
- Visualized numerical feature distributions using KDE plots.
- Created a heatmap to observe correlations between variables.
- Analyzed target variable (life_expectancy) with histograms and boxplots.

### 3. Feature Selection
- Calculated VIF to identify multicollinearity.
- Used two methods for feature importance:
  - RandomForestRegressor: Found top features as income_composition_of_resources, hiv/aids, and adult_mortality.
  - LinearRegression with SelectKBest: Provided an alternate set of contributing features.
- Final feature selection: income_composition_of_resources, hiv/aids, adult_mortality, thinness_1-19_years, schooling, and bmi.

### 4. Modeling
- Applied and compared multiple regression models:
  - Linear Regression
  - Ridge Regression
  - Random Forest Regressor
  - XGBoost Regressor
- Evaluated using:
  - R² Score
  - RMSE
  - 5-Fold Cross-Validation

### 5. Results
- Best model: Random Forest Regressor
  - R²: 0.9676
  - RMSE: 2.80
  - Cross-Val Mean R²: 0.9181
- Residuals showed a consistent pattern with no major heteroscedasticity.
- XGBoost also performed well (R²: 0.9646), but Random Forest had slightly better overall metrics.

### 6. Model Saving
Saved the final trained Random Forest model using joblib for future deployment.

## Final Notes:
- The project demonstrates the importance of feature selection and proper preprocessing.
- Random Forest provided strong predictive performance with minimal tuning.
- Feature scaling was carefully addressed during modeling.
