Global Cars Data Analysis Project
This project focuses on performing an Exploratory Data Analysis (EDA) on a comprehensive dataset of global cars. It aims to uncover trends in the automotive industry, analyze pricing factors, and evaluate engine performance and fuel efficiency across different brands and manufacturing countries.

📁 Repository Structure
global_cars_enhanced.xlsx: The primary dataset containing detailed specifications of various car models.

lab3.ipynb: A Jupyter Notebook containing the complete Python workflow, including data cleaning, preprocessing, and visualization.

📊 Dataset Overview
The dataset includes several key features for analysis:

Car Identification: Car_ID, Brand, Manufacturing_Country.

Technical Specs: Engine_CC, Horsepower, Transmission, Fuel_Type, Body_Type.

Performance: Mileage_km_per_l, Efficiency_Score, HP_per_CC.

Market Data: Price_USD, Manufacture_Year, Car_Age, Price_Category.

🛠 Project Workflow
The analysis in the notebook follows these steps:

1. Data Cleaning & Preprocessing
Header Correction: Fixed issues where the first row of the Excel file was treated as data.

Handling Missing Values: Checked for null values and duplicates to ensure data integrity.

Type Conversion: Converted relevant columns (Price, Horsepower, Year, etc.) into numeric formats for calculation.

2. Descriptive Statistics
Generated a statistical summary (Mean, Median, Std Dev) for all numerical features to understand the data distribution.

3. Data Visualization (EDA)
Univariate Analysis:

Distribution of car prices to identify market segments.

Distribution of Horsepower to understand engine performance trends.

Bivariate Analysis:

Average car price based on Fuel Type.

Comparison of car prices across different Brands.

Relationship between car age and pricing.

🚀 Getting Started
To run this project locally, follow these steps:

Clone the repository:

Bash
git clone https://github.com/your-username/global-cars-analysis.git
Install dependencies:

Bash
pip install pandas numpy matplotlib seaborn openpyxl
Run the Notebook:
Open lab3.ipynb using Jupyter Notebook or VS Code to view the analysis and charts.

📈 Key Insights
Identify which brands dominate the luxury vs. budget categories.

Analysis of how fuel type (Petrol, Diesel, Hybrid, etc.) affects the resale value and price.

Correlation between engine size (CC) and fuel efficiency.

Suggested GitHub Topics:
python data-analysis eda matplotlib seaborn automotive-data pandas
