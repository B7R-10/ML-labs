ARTI308 – Lab 11: Credit Card Customer Segmentation Using K-Means

Overview

This lab demonstrates how to build and evaluate a K-Means clustering model using Python.
The objective is to segment credit card customers based on their financial behavior and usage patterns.
Dataset used: Credit Card Customer Dataset (CC_GENERAL.csv)

The notebook covers the following steps:

Data loading

Data exploration

Data cleaning

Exploratory data analysis (EDA)

Feature scaling

K-Means clustering

Choosing the optimal number of clusters

Cluster visualization using PCA

Cluster interpretation

Files Included

LAB 11.ipynb

Main Jupyter Notebook containing the full lab solution.

CC_GENERAL.csv

Dataset used for customer segmentation.

README.md

Description of the project and instructions on how to run the notebook.

Requirements

Make sure the following Python libraries are installed:

pandas

numpy

matplotlib

seaborn

scikit-learn

Install them using:

pip install pandas numpy matplotlib seaborn scikit-learn

How to Run the Notebook

Open the notebook in Jupyter Notebook or Google Colab.

Make sure the file CC_GENERAL.csv is in the same folder as the notebook.

Run all cells from top to bottom.

In Jupyter Notebook:

Run → Run All Cells

Machine Learning Model

Model used in this lab:

K-Means Clustering

This project is an unsupervised learning task because the dataset does not contain predefined labels.
The model groups customers into clusters based on similarities in their behavior.

Features used for clustering include:

BALANCE

PURCHASES

CASH_ADVANCE

CREDIT_LIMIT

PAYMENTS

MINIMUM_PAYMENTS

PRC_FULL_PAYMENT

TENURE

and other customer behavior variables

Data Cleaning

The following preprocessing steps were performed:

Removed the CUST_ID column because it is only an identifier.

Checked for missing values.

Filled missing values using mean imputation.

Applied feature scaling using StandardScaler.

Exploratory Data Analysis (EDA)

The notebook includes several visualizations to better understand the dataset:

Histograms for numerical features

Correlation heatmap

Scatter plot of BALANCE vs PURCHASES

Scatter plot of BALANCE vs CASH_ADVANCE

These visualizations help identify customer behavior patterns and relationships between variables.

Choosing the Number of Clusters

Two techniques were used to determine the best number of clusters:

Elbow Method

The elbow method compares inertia values for different K values.

Silhouette Score

The silhouette score measures how well-separated the clusters are.

The final K value was selected based on these evaluation methods.

Cluster Visualization

Since the dataset contains many features, PCA (Principal Component Analysis) was used to reduce the dimensions to 2 components.

A scatter plot was then created to visualize the customer clusters.

Evaluation and Interpretation

After clustering:

Customers were grouped into different segments.

Cluster centers were analyzed.

The average behavior of customers in each cluster was interpreted.

This helps businesses better understand different customer types and improve marketing strategies.

Conclusion

A K-Means clustering model was built to segment credit card customers based on their spending and payment behavior.
The dataset was cleaned, scaled, and analyzed using multiple visualizations.
The optimal number of clusters was selected using the elbow method and silhouette score.
Finally, PCA was used to visualize the customer groups and interpret their behavior.

Author

Saleh Albahr


