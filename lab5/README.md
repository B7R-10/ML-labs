# ARTI308 Lab 5

## Overview

This lab focuses on applying **feature engineering techniques** to improve machine learning model performance using a food delivery dataset.

The dataset contains information about orders such as item name, quantity, total price, order time, and order status.

## Dataset

The dataset used in this project is **talabat_enhanced_orders.csv**, which includes information about customer orders and delivery details.

## Tasks

### Task 1 – Feature Engineering

A new feature called **price_per_item** was created by dividing the total price by the quantity. This helps the model understand the average cost of items in each order.

### Task 2 – Peak Hour Feature

Peak hours were defined as **11–14** (lunch) and **18–21** (dinner). This feature helps capture periods of high order demand.

### Task 3 – Item Reduction

The **Item_Name** feature was simplified using the **top_k approach**, where only the most frequent items are kept and the rest are grouped as **Other**.

### Task 4 – Feature Selection

Feature selection was applied using **SelectKBest** to identify the most important features for predicting the order status.

## Tools Used

* Python
* Pandas
* Scikit-learn
* Jupyter Notebook

## Author

Saleh Albahr

