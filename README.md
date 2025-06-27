# 📊 PromoCast: Sales Forecasting for Rossmann Stores using Random Forest

**PromoCast** is a machine learning project that forecasts daily sales for Rossmann retail stores using historical data and store metadata. It applies a **Random Forest Regressor** with hyperparameter tuning to build an accurate and interpretable sales prediction model.

---

## 📁 Dataset

- Source: [Rossmann Store Sales Dataset (Kaggle)](https://www.kaggle.com/c/rossmann-store-sales)
- Contains:
  - Daily sales data for 1,000+ stores
  - Promotion details, holidays, assortment levels
  - Metadata such as store type and competition distance

---

## 🚀 Features

- Merges transactional and store metadata
- Cleans and filters only relevant sales data
- Extracts time-based features (`Year`, `Month`, `WeekOfYear`, etc.)
- Encodes categorical variables using one-hot encoding
- Tunes model with `RandomizedSearchCV` and cross-validation
- Evaluates performance with MAE, RMSE, R²
- Visualizes predictions, residuals, and feature importances

---

## Workflow
- 1. Load train.csv and store.csv
- 2. Merge on 'Store'
- 3. Filter: Open stores with non-zero sales
- 4. Feature Engineering:
    - Date-based features
    - Weekend and Promo*Holiday interactions
- 5. One-hot encode categorical columns
- 6. Train/test split (80/20)
- 7. Fit Random Forest with RandomizedSearchCV
- 8. Evaluate using MAE, RMSE, R²
- 9. Visualize outputs and feature importance
