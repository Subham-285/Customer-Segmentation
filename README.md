# Customer-Segmentation
# Project Overview
Customer segmentation is the process of grouping customers based on similar characteristics, purchasing behavior, and engagement patterns.

This project performs Exploratory Data Analysis (EDA) and applies unsupervised machine learning clustering techniques to identify meaningful customer groups from demographic, purchasing, campaign, and engagement data.

The analysis explores customer characteristics such as income, education, marital status, purchasing behavior, product spending, website activity, campaign responses, and recency of purchase.

# Objectives
- Understand customer demographics and purchasing behavior.
- Clean and preprocess customer-level data.
- Analyze spending and purchasing patterns through EDA.
- Engineer relevant features for customer segmentation.
- Apply different clustering algorithms.
- Visualize the resulting customer groups.
- Compare different approaches to unsupervised segmentation.

# Exploratory Data Analysis
The project investigates several dimensions of customer behavior:

# Demographic Analysis
- Customer birth-year distribution
- Education levels
- Marital status
# Income Analysis
- Income distribution
- Descriptive statistics
IQR-based outlier filtering
# Family Characteristics
- Number of children
- Number of teenagers


# Customer Registration
The Dt_Customer field is transformed into:
- Dt_day
- Dt_month
- Dt_year
# Customer Engagement
- Recency of customer activity
- Website visits
- Purchase channels
# Product Spending
Customer spending is analyzed across:
- Wine
- Fruits
- Meat products
- Fish products
- Sweet products
- Gold products
# Marketing Campaign Analysis

The project analyzes customer acceptance across five marketing campaigns and the final campaign response.

# Customer Complaints

The proportion of customers who submitted complaints is also examined.

# Data Preprocessing
The following preprocessing steps were performed:

1. Loaded the customer dataset using Pandas.
2. Inspected data types and missing values.
3. Checked for duplicate records.
4. Imputed missing Income values using the median.
5. Converted the customer registration date into separate day, month, and year features.
6. Removed the original ID and Dt_Customer fields from the modeling dataset.
7. Encoded categorical variables:
   Education
   Marital_Status
8. Created an aggregate purchasing feature.

# Feature Engineering
A new feature called Purchases was created by combining spending across all six product categories:

Purchases =
MntWines
+ MntFruits
+ MntMeatProducts
+ MntFishProducts
+ MntSweetProducts
+ MntGoldProds

This provides an overall measure of customer spending across product categories.

The relationship between Income and Purchases was also visualized before clustering.
