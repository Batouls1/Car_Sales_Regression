# Car Price Prediction using Machine Learning

This project builds and evaluates regression models to predict **car prices** based on various numerical and categorical features.  
It includes data preprocessing, model comparison, and performance evaluation.

---

## Project Overview

- **Goal:** Predict car selling prices using supervised machine learning.
- **Techniques Used:**
  - Data preprocessing with 'ColumnTransformer' and 'Pipeline'
  - Encoding categorical features and scaling numerical ones
  - Model training & comparison ('Ridge', 'SVR', 'RandomForest')
  - Evaluation using regression metrics ('R2', 'MAE', 'MSE')

---

## Workflow Summary

1. **Data Exploration & Cleaning**  
   - Checked for missing values and data distributions.  
   - Applied log transformation to stabilize target variance.

2. **Feature Engineering & Preprocessing**  
   - Scaled numerical features and encoded categorical ones.  
   - Built a pipeline for consistent preprocessing and training.

3. **Model Training & Evaluation**  
   - Compared multiple models (Ridge, SVR, Random Forest).  
   - Selected **Ridge Regression** as best performer with:
     - R² = 0.21  
     - MSE = 0.24  
     - MAE = 0.40  

---

## Interpretation

The relatively low R2 indicates limited predictive power due to the **small dataset size and limited feature variety**.  
With more data and richer features (e.g., car age, engine type, fuel efficiency), the model’s accuracy would likely improve.

---

## Tech Stack

- Python  
- Scikit-learn  
- Pandas  
- NumPy  
- Matplotlib / Seaborn (for visualization)

---

## Results Example

Sample predicted prices (after reversing log transform):

[16508.00192431, 20434.88362276, 10397.05882459,  7946.59726899,
 8944.34964389, 10372.76659618, 13654.82935156, 11987.12526432,
 17643.9521231 , 12666.77083855,  7805.40488742, 14691.35873185,
 10931.52474892, 12338.55592261, 12769.35672229, 14525.62109194,
 14028.9191593 ,  9844.37733339, 10647.29709781, 10661.2181954]


## How to Use

1. **Install Dependencies**:
Make sure you have Python 3.x installed, then run:
```bash
    pip install -r requirements.txt
```
2. **Run the Notebook**:
Launch Jupyter and open the main notebook file:
```bash
    jupyter notebook car_sales_regression.ipynb
```

3. **Run All Cells**:
Execute all cells in order (Kernel -> Restart & Run All) to reproduce the results.    

Notes:

- Replace any placeholder paths (e.g., 'data/car-sales-data.csv') with your actual dataset location.

- Ensure all necessary data files are available in the correct directories before running.
