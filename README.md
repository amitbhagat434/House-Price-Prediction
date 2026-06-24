# House Price Prediction using Linear Regression

A simple machine learning project that predicts house prices based on features like area, bedrooms, bathrooms, location, and condition using **Linear Regression**.

## Dataset
The dataset (`House_Price_Prediction_Dataset.csv`) contains the following features:
- `Area`, `Bedrooms`, `Bathrooms`, `Floors`, `YearBuilt`
- `Location` (Rural/Suburban/Urban/Downtown)
- `Condition` (Poor/Fair/Good/Excellent)
- `Garage` (Yes/No)
- `Price` (target variable)

## Workflow
1. **Data Cleaning** – Checked for nulls, duplicates, and data types
2. **Feature Encoding** – Converted categorical columns to numeric:
   - `Garage`: Yes → 1, No → 0
   - `Location`: Rural → 0, Suburban → 1, Urban → 2, Downtown → 3
   - `Condition`: Poor → 0, Fair → 1, Good → 2, Excellent → 3
3. **EDA** – Correlation heatmap, pairplots, boxplots, and distribution plots
4. **Preprocessing** – Train-test split (80/20) and feature scaling with `StandardScaler`
5. **Model Training** – Fitted a `LinearRegression` model from scikit-learn
6. **Evaluation** – Compared actual vs predicted prices, plotted regression line, and computed **R² Score**

## Tech Stack
- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Results
The model predicts house prices with an R² score printed at the end of the notebook, along with visualizations comparing actual vs predicted values.

## How to Run
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
jupyter notebook House_Price_Prediction_using_Linear_Regression.ipynb
```

## 📁 Files
- `House_Price_Prediction_using_Linear_Regression.ipynb` – Main notebook
- `House_Price_Prediction_Dataset.csv` – Dataset
