# Retail Sales & Customer Analytics Dashboard

## Project Overview
This project analyzes retail sales, profitability, product performance, customer segments, and regional performance using Microsoft Power BI.

The goal is to transform raw retail data into an interactive dashboard that helps identify business trends and support data-driven decisions.

## Dataset
- **Dataset:** Sample Superstore
- **Source:** [Kaggle - Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- **Records:** 9,994 rows
- **Columns:** 21
- **Date Range:** January 2014 – December 2017

## Tools & Technologies
- Microsoft Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Data Visualization

## Data Preparation
- Imported the dataset into Power BI.
- Checked data types and column quality.
- Verified missing values and duplicate records.
- Changed Postal Code to Text data type.
- Created calculated columns for Year-Month analysis.
- Created DAX measures for key business metrics.

## Dashboard Pages

### 1. Sales Overview
- Total Sales
- Total Profit
- Profit Margin
- Total Orders
- Monthly Sales Trend
- Sales by Category
- Sales and Profit by Region

### 2. Product Analysis
- Total Products
- Total Categories
- Total Sub-Categories
- Top 10 Products by Sales
- Top 10 Products by Profit
- Bottom 10 Products by Profit
- Sales by Sub-Category

### 3. Customer & Regional Analysis
- Total Customers
- Total Customer Segments
- Total Regions
- Sales by Customer Segment
- Profit by Customer Segment
- Top 10 Customers by Sales
- Sales by Region
- Sales by State Map

## Key Business Insights

- Technology generated the highest sales among the three product categories.
- The West region recorded the highest sales among all regions.
- Consumer customers contributed approximately 50.56% of total sales.
- Furniture generated considerably lower profit compared with Technology and Office Supplies.
- The dashboard highlights products with both high and low profitability.

## Key DAX Measures

```dax
Total Sales = SUM('Sample - Superstore'[Sales])

Total Profit = SUM('Sample - Superstore'[Profit])

Profit Margin = DIVIDE([Total Profit], [Total Sales], 0)

Total Orders = DISTINCTCOUNT('Sample - Superstore'[Order ID])

Total Customers = DISTINCTCOUNT('Sample - Superstore'[Customer ID])

Total Products = DISTINCTCOUNT('Sample - Superstore'[Product ID])
```

## Interactive Features
- Date range slicer
- Region slicer
- Category slicer
- Cross-filtering between visuals
- Interactive charts and KPI cards

## Conclusion
This project demonstrates the use of Power BI for data preparation, DAX calculations, interactive dashboard development, and business analysis. It provides insights into sales performance, customer behavior, product profitability, and regional trends.

