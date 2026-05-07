# CIS307 – Lab 10: Support Vector Machines (SVM)

## Overview
This lab demonstrates how to build and evaluate a Support Vector Machine (SVM) classifier using Python.
The objective is to classify iris flower species based on their physical measurements.
Dataset used: Iris Flower Dataset (loaded via Seaborn)

The notebook covers the following steps:
- Data loading
- Data exploration
- Exploratory data analysis (EDA)
- Train/Test split
- Model training
- Prediction
- Model evaluation
- Gridsearch parameter tuning

---

## Files Included
02-SVM_Assignment.ipynb
Main Jupyter Notebook containing the full lab solution.

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
2. Run all cells from top to bottom.

In Jupyter Notebook:
Run → Run All Cells

---

## Machine Learning Model
Model used in this lab:
Support Vector Machine (SVC)

Features used for classification:
sepal_length
sepal_width
petal_length
petal_width

Target variable:
species (setosa / versicolor / virginica)

---

## Evaluation Metrics
The following metrics are used to evaluate the model:

Confusion Matrix
Classification Report (Precision, Recall, F1-Score)

These metrics help measure how accurately the model classifies each flower species.

---

## Visualizations
The notebook includes two main visualizations:

1. Pairplot of all features colored by species
2. KDE plot of sepal_length vs sepal_width for Setosa species

These plots help understand the data distribution and species separability.

---

## GridSearch Tuning
GridSearchCV was used to find the best hyperparameters for the SVM model.

Parameters tested:
C: [0.1, 1, 10, 100]
gamma: [1, 0.1, 0.01, 0.001]

---

## Conclusion
A Support Vector Machine (SVM) classifier was trained to predict iris flower species
using sepal and petal measurements. The model was evaluated using a confusion matrix
and classification report, and further tuned using GridSearchCV to optimize performance.

---

## Author
Saleh Albahr
