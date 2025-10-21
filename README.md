# Chocolate Sales Prediction with Machine Learning

This project explores and models chocolate sales data using machine learning techniques. It includes a full data science workflow from data exploration and preprocessing to predictive modeling and evaluation.

## Dataset

- **Source**: [Kaggle - Chocolate Sales Dataset](https://www.kaggle.com/datasets/atharvasoundankar/chocolate-sales)
- **Records**: 1094
- **Features**: Sales Person, Country, Product, Date, Amount (target), Boxes Shipped

## Project Structure

1. **Data Loading and Preprocessing**
   - Importing libraries
   - Reading and cleaning the dataset
   - Handling currencies and dates
   - Feature engineering (e.g. extracting date parts)
   - One-hot encoding of categorical features

2. **Exploratory Data Analysis (EDA)**
   - Visual analysis by product, country, month, day of week, and salesperson
   - Distribution analysis of the target variable (`amount`)
   - Business insights on top products and performers

3. **Modeling**
   - Feature selection and data splitting
   - Training Random Forest and Gradient Boosting models
   - Hyperparameter tuning (tree depth)
   - Evaluation using MAE, RMSE, and R² metrics

4. **Results**
   - Best performance: **Random Forest Regressor** with depth = 5  
   - **MAE** ≈ 3256  
   - **RMSE** ≈ 4071  
   - **R²** ≈ -0.02

5. **Insights**
   - Top products: *Smooth Silky Salty*, *50% Dark Bites*
   - Best-performing countries: *Australia*, *UK*, *India*, *USA*
   - Most successful salespersons: *Chess Bonnell*, *Oby Sorrel*
   - Sales mostly occurred on weekdays, with *Thursday* and *Tuesday* being strongest

## Key Takeaways

- The models struggled to accurately predict `amount`, often regressing to the mean.
- Feature importance suggests that `boxes shipped` is the strongest predictor.
- Further improvements require more features or external data (e.g. marketing efforts, seasonality, prices).

## Files

- `notebook.ipynb` — Main analysis and modeling notebook
- `README.md` — Project description and structure

## Technologies Used

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook
- Random Forest & Gradient Boosting Regressors

## Future Improvements

- Add external data sources to enrich features
- Try advanced models like XGBoost or LightGBM
- Build a web dashboard for interactive analysis

---

**Author**: Nadya Antonova  
**Date**: October 2025
