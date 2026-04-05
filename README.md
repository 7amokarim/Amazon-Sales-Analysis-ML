# Amazon Sales Analysis and Prediction

## Overview
This project focuses on analyzing an Amazon products dataset to understand the key factors that influence sales and to build machine learning models capable of predicting total sales. The work combines data analysis, statistical testing, and predictive modeling in a complete end-to-end pipeline.

---

## Objectives
The main goals of this project are:
- Analyze product data to extract meaningful insights
- Understand the relationship between price, ratings, and sales
- Perform statistical tests to validate assumptions
- Build and evaluate machine learning models for prediction

---

## Dataset Description
The dataset contains information about Amazon products, including:
- Product ID and name
- Category
- Discounted price and actual price
- Discount percentage
- Rating and rating count
- Product descriptions and reviews

---

## Data Preprocessing
Several preprocessing steps were applied to ensure data quality:
- Handling missing values in both numerical and categorical columns
- Converting data types (e.g., prices from text to numeric)
- Encoding categorical variables using one-hot encoding and label encoding
- Scaling numerical features using standardization

---

## Feature Engineering
New features were created to improve analysis and model performance:
- Total_Sale: derived from price assumptions
- Profit: estimated based on total sale
- Additional transformed features such as normalized values

Note: Features directly derived from the target variable were excluded from model training to avoid data leakage.

---

## Exploratory Data Analysis (EDA)
The analysis phase included:
- Distribution plots for numerical variables
- Boxplots to detect outliers
- Correlation heatmaps to understand relationships
- Pairplots to visualize interactions between features

---

## Outlier Detection
Outliers were identified using the Z-score method. Data points exceeding a threshold were visualized and analyzed to understand their impact on the dataset.

---

## Statistical Testing
Two statistical methods were used:

### Independent T-Test
Used to compare sales between high-sale and low-sale groups.

### ANOVA Test
Used to determine whether there are significant differences in sales across product categories.

Both tests showed statistically significant differences, supporting the hypotheses.

---

## Machine Learning Models

### 1. Linear Regression
Used as a baseline model to understand linear relationships between features and total sales.

### 2. Random Forest Regressor
A more advanced model capable of capturing non-linear relationships and feature interactions.

---

## Model Evaluation
Models were evaluated using:
- RMSE (Root Mean Squared Error)
- R² Score

Random Forest achieved better performance compared to Linear Regression, indicating its ability to model complex patterns.

---

## Feature Importance
Feature importance analysis using Random Forest revealed:
- Price-related features have the strongest impact on sales
- Discount percentage has relatively low influence
- Ratings have minimal effect on total sales

---

## Key Insights
- Higher prices are strongly associated with higher total sales
- Discounts do not significantly increase sales
- Ratings and review counts have limited impact on sales performance
- Pricing strategy plays a more critical role than promotional discounts

---

## Technologies Used
- Python
- Pandas and NumPy for data manipulation
- Matplotlib and Seaborn for visualization
- Scikit-learn for machine learning

