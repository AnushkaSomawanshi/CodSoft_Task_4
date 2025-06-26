# CODSOFT Internship Projects

This repository includes the work I completed as part of the CODSOFT Data Science Internship.  
Each task focuses on solving real-world problems using Python and machine learning techniques.  

This README describes **Task 4: Sales Prediction Using Python**.

---

# Task 4: Sales Prediction Using Python

## Project Overview

This project focuses on forecasting product sales using machine learning regression techniques.  
Accurate sales predictions help businesses optimize marketing strategies, allocate budgets wisely, and improve ROI.  

By analyzing historical data that includes advertising budgets across various platforms (TV, Radio, Newspaper),  
the model is trained to predict future sales values based on budget distribution.

---

## What I Did

- Loaded and explored a dataset with sales and advertising budget data  
- Performed data cleaning and preprocessing  
- Conducted Exploratory Data Analysis (EDA) to identify trends and correlations  
- Applied regression models to predict future sales:
  - Linear Regression  
  - Random Forest Regressor  
- Evaluated model performance using Mean Squared Error and R-squared score  
- Created a sample prediction setup to simulate sales forecasting

---

## What I Observed

- TV advertising had the most significant positive influence on sales  
- Radio had a moderate effect, while Newspaper advertising had the least impact  
- Random Forest Regressor outperformed Linear Regression in prediction accuracy  
- Visualizations helped confirm trends and feature importance  
- Slight budget increases in TV and Radio showed noticeable improvements in sales prediction

---

## Dataset Description

The dataset used in this project contains the following columns:

- `TV`: Budget spent on TV advertisements (in thousands of dollars)  
- `Radio`: Budget spent on Radio advertisements  
- `Newspaper`: Budget spent on Newspaper advertisements  
- `Sales`: Sales of the product (target variable)

---

## Key Steps in the Project

### 1. Data Preprocessing

- Loaded data into a pandas DataFrame  
- Checked for null, missing, and duplicate entries  
- Ensured data types and formatting were correct

### 2. Exploratory Data Analysis (EDA)

- Created scatter plots and correlation heatmaps  
- Analyzed relationships between advertising channels and sales  
- Identified multicollinearity and distribution trends

### 3. Model Training

- Split data into training and test sets using `train_test_split`  
- Trained two models:
  - Linear Regression  
  - Random Forest Regressor

### 4. Evaluation

- Used metrics such as:
  - Mean Squared Error (MSE)  
  - R² Score (R-squared)  
- Visualized predicted vs actual sales using plots

---

## Sample Prediction

```python
import pandas as pd

# Example input
sample_data = pd.DataFrame({
    'TV': [150],
    'Radio': [30],
    'Newspaper': [20]
})

# Predict sales
predicted_sales = model.predict(sample_data)
print("Predicted Sales:", round(predicted_sales[0], 2))
