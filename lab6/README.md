# ARTI308 – Lab 6: Linear Regression

## Overview
This lab demonstrates how to build and evaluate a Linear Regression model using Python.  
The objective is to predict car prices based on several vehicle features from the dataset.

Dataset used: global_cars_enhanced.xlsx

The notebook covers the following steps:
- Data loading
- Data exploration
- Data cleaning
- Feature selection
- Model training
- Prediction
- Model evaluation
- Visualization

---

## Files Included

ARTI308_Lab6_NoErrors.ipynb  
Main Jupyter Notebook containing the full lab solution.

global_cars_enhanced.xlsx  
Dataset used for training and testing the model.

README.md  
Description of the project and instructions on how to run the notebook.

---

## Requirements

Make sure the following Python libraries are installed:

pandas  
numpy  
matplotlib  
seaborn  
scikit-learn

Install them using:

pip install pandas numpy matplotlib seaborn scikit-learn

---

## How to Run the Notebook

1. Open the notebook in Jupyter Notebook or Google Colab.
2. Place the dataset file "global_cars_enhanced.xlsx" in the same folder as the notebook.
3. Run all cells from top to bottom.

In Jupyter Notebook:

Run → Run All Cells

---

## Machine Learning Model

Model used in this lab:

Linear Regression

Features used for prediction:

Engine_CC  
Horsepower  
Mileage_km_per_l  
Car_Age  
HP_per_CC  
Efficiency_Score  

Target variable:

Price_USD

---

## Evaluation Metrics

The following metrics are used to evaluate the model:

Mean Absolute Error (MAE)  
Mean Squared Error (MSE)  
Root Mean Squared Error (RMSE)

These metrics help measure how accurate the model predictions are compared to the actual car prices.

---

## Visualizations

The notebook includes two main visualizations:

1. Actual vs Predicted Prices scatter plot  
2. Residual distribution plot

These plots help understand the model performance and prediction errors.

---

## Conclusion

A Linear Regression model was trained to predict car prices using several car features.  
The model was evaluated using different metrics and visualizations to assess its performance.

---

## Author

Saleh Albahr
