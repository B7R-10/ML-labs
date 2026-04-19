Global Cars Advanced Data Analysis
This project performs an advanced Exploratory Data Analysis (EDA) and Feature Engineering on a global car dataset. It covers everything from data quality assessment to advanced dimensionality reduction techniques to understand the complex relationships in the automotive market.

📁 Repository Structure
global_cars_enhanced.xlsx: The core dataset featuring specifications of diverse car models.

lab4.ipynb: An advanced Jupyter Notebook containing the full pipeline, including data quality checks, Z-score normalization, and Principal Component Analysis (PCA).

📊 Dataset Overview
The analysis utilizes a rich set of features:

Vehicle Information: Brand, Body_Type, Fuel_Type, Transmission.

Technical Specs: Engine_CC, Horsepower, HP_per_CC.

Market & Performance: Price_USD, Mileage_km_per_l, Efficiency_Score, Car_Age.

🛠 Project Workflow
The analysis is divided into several specialized tasks:

1. Data Quality & Cleaning
Issue Identification: Detecting noise, missing values, and structural inconsistencies.

Data Refining: Cleaning headers and ensuring all technical columns are in the correct numeric format for mathematical modeling.

2. Feature Transformation & Scaling
Z-Score Normalization: Standardizing features like Price_USD and Horsepower using StandardScaler to bring them to a common scale, which is essential for advanced algorithms.

Handling Outliers: Analyzing data distribution to ensure robust results.

3. Advanced Dimensionality Reduction (PCA)
Principal Component Analysis: Applied PCA to reduce the complexity of the data while preserving maximum variance.

Variance Analysis: Explained how much information (variance) is captured by the principal components (e.g., analyzed the Explained Variance Ratio for Price and Horsepower).

4. Statistical & Visual Exploration
Distribution Analysis: Visualizing the spread of prices and engine power using Seaborn and Matplotlib.

Correlation Studies: Investigating how technical specifications influence the market value and fuel efficiency.

📈 Key Technical Insights
PCA Results: Identified the primary factors that drive the differences between car models.

Market Segmentation: Clear distinction between budget, mid-range, and luxury categories based on normalized performance metrics.

Efficiency Trends: Insights into how manufacturing origin affects the "Efficiency Score" of modern vehicles.
