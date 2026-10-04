# SWYNEX Exploratory Data Analysis

## Project Overview

This project was completed as part of my Data Analyst Internship at SWYNEX Technologies.

The objective of this task was to perform Exploratory Data Analysis (EDA) on a cleaned Cafe Sales dataset and identify useful trends, patterns, relationships, and data-quality issues.

The analysis was performed using Python and popular data analysis and visualization libraries.

## Dataset

The dataset contains 10,000 cafe sales transactions with the following columns:

- Transaction ID
- Item
- Quantity
- Price Per Unit
- Total Spent
- Payment Method
- Location
- Transaction Date

The cleaned dataset was prepared during Task 1: Data Cleaning & Preparation.

## Objectives

The main objectives of this EDA project were:

- Understand the structure of the dataset
- Calculate important descriptive statistics
- Analyze item-wise sales and revenue
- Analyze payment methods
- Analyze revenue by location
- Identify monthly revenue trends
- Examine high-value transactions
- Analyze the relationship between quantity and total spending
- Identify data-quality issues
- Generate useful business insights

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

## Exploratory Data Analysis Performed

### 1. Dataset Overview

The dataset contains:

- 10,000 transactions
- 8 columns

Descriptive statistics and missing-value checks were also performed.

### 2. Item-wise Quantity Analysis

Coffee was the top-selling item by quantity, with:

**3,534 units sold**

### 3. Revenue by Item

Salad generated the highest item-level revenue:

**17,320**

### 4. Payment Method Analysis

The analysis showed that the `Unknown` category had the highest number of transactions:

**3,178 transactions**

This indicates a significant data-quality issue because `Unknown` does not represent an actual payment method.

### 5. Location Analysis

The `Unknown` location category recorded the highest revenue:

**35,337.5**

Since this is not an actual location, reliable location-based conclusions are limited.

### 6. Monthly Revenue Analysis

Monthly revenue during the available period was:

| Month | Revenue |
|---|---:|
| January 2023 | 7,242.0 |
| February 2023 | 6,633.5 |
| March 2023 | 7,214.5 |
| April 2023 | 7,168.0 |
| May 2023 | 6,941.5 |

Revenue fluctuated during the period, with January recording the highest monthly revenue and February recording the lowest.

### 7. Quantity vs Total Spent

The correlation between Quantity and Total Spent was:

**0.7041**

This indicates a fairly strong positive relationship between the quantity purchased and the total transaction value.

## Key Business Insights

1. **Coffee was the top-selling item**, with 3,534 units sold, indicating strong demand for this product.

2. **Salad generated the highest item-level revenue**, reaching 17,320.

3. **Monthly revenue fluctuated** during January–May 2023, ranging from 6,633.5 to 7,242.0.

4. **Quantity and Total Spent showed a positive correlation of approximately 0.704**, meaning higher quantities purchased were generally associated with higher transaction values.

5. **Payment-method data contains a significant number of Unknown values**, with 3,178 transactions, highlighting an important data-quality limitation.

6. **Location data also contains Unknown values**, which limits the reliability of location-level revenue comparisons.

## Visualizations

The analysis includes visualizations for:

- Quantity Sold by Item
- Revenue by Item
- Transactions by Payment Method
- Revenue by Location
- Monthly Revenue Trend
- Distribution of Transaction Values
- Quantity vs Total Spent

## Conclusion

The Exploratory Data Analysis provided useful insights into product performance, revenue patterns, transaction behavior, and data quality.

Coffee showed the highest sales volume, while Salad generated the highest item-level revenue. The positive correlation between quantity and total spending indicates that transaction value generally increases as customers purchase more items.

The analysis also identified significant `Unknown` values in payment-method and location fields. Improving these data fields would allow more reliable business analysis and decision-making.

## Project Structure

```text
SWYNEX-Exploratory-Data-Analysis
│
├── Data
│   └── cleaned_cafe_sales.csv
│
├── notebooks
│   └── EDA_Cafe_Sales.ipynb
│
└── README.md