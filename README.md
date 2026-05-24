# Retail Black Friday Sales Data Engineering Project

## Project Overview

This project demonstrates an end-to-end retail data engineering and analytics workflow using Python, pandas, Google Colab, and a Kaggle Black Friday sales dataset.

The project processes raw retail transaction data and creates business-ready analytical outputs such as KPI tables, customer summaries, category-level reports, RFM customer segmentation, and suspicious transaction reports.

## Dataset

Dataset file used:

`retail_black_friday_sales_100k.csv`

Source:

Kaggle — Black Friday Sales Dataset  
https://www.kaggle.com/datasets/noopurbhatt/retail-black-friday-sales-dataset?select=retail_black_friday_sales_100k.csv

The CSV file is included in this repository for reproducibility.

## Repository Structure

```text
retail-black-friday-sales-data-engineering/
│
├── retail_black_friday_sales_data_engineering_project.ipynb
├── retail_black_friday_sales_100k.csv
└── README.md
```

## Objectives

- Load raw retail transaction data
- Inspect schema, nulls, duplicates, and data types
- Clean and transform the dataset
- Create date and business features
- Generate business KPI tables
- Perform customer-level analysis
- Build RFM customer segmentation
- Detect suspicious transactions
- Export analytics-ready CSV outputs

## Tools Used

- Python
- pandas
- NumPy
- Google Colab
- Kaggle dataset

## Dataset Columns

- transaction_id
- customer_id
- age_group
- gender
- city
- customer_segment
- product_id
- product_category
- original_price
- discount_pct
- final_price
- quantity
- purchase_amount
- payment_method
- purchase_date
- purchase_hour
- is_weekend
- is_black_friday

## Analysis Performed

### 1. Top Selling Product Categories

Identified product categories generating the highest revenue, quantity sold, and transaction count.

### 2. Revenue by City

Analyzed which cities contributed the most revenue and customer activity.

### 3. Payment Method Analysis

Compared payment methods by usage, revenue, average order value, and transaction percentage.

### 4. Weekend vs Weekday Sales

Compared revenue and order behavior between weekends and weekdays.

### 5. Customer Segment Analysis

Analyzed revenue, order count, unique customers, and average order value across customer segments.

### 6. Discount Impact Analysis

Created discount buckets and analyzed how discount levels affected revenue, order count, and average order value.

### 7. Hourly Sales Trend

Analyzed revenue and transaction patterns by purchase hour.

### 8. Age Group and Category Analysis

Studied how different age groups spend across product categories.

### 9. Black Friday vs Normal Day Sales

Compared Black Friday sales performance against normal day sales.

### 10. KPI Table

Created a business summary table containing:

- Total revenue
- Total transactions
- Unique customers
- Unique products
- Average order value
- Total quantity
- Average discount percentage

### 11. Customer Summary Table

Created one row per customer with:

- Total transactions
- Total spend
- Average order value
- Total quantity
- First purchase date
- Last purchase date
- Preferred city
- Preferred category
- Preferred payment method

### 12. RFM Analysis

Built customer segmentation using:

- Recency
- Frequency
- Monetary value

Assigned customers into segments such as:

- Best Customers
- Loyal Customers
- At Risk
- New / Recent Customers
- Others

### 13. Suspicious Transaction Detection

Detected suspicious transactions using rule-based logic:

- High discount
- High quantity
- High purchase amount
- Late-night purchase

## Key Outputs

The notebook exports the following analytics-ready CSV files:

- top_categories.csv
- city_revenue.csv
- payment_analysis.csv
- weekend_sales.csv
- segment_analysis.csv
- discount_analysis.csv
- hourly_sales.csv
- age_category_sales.csv
- black_friday_analysis.csv
- kpi_table.csv
- customer_summary.csv
- rfm_analysis.csv
- suspicious_transactions.csv

## Skills Demonstrated

- Data ingestion
- Data cleaning
- Data transformation
- Feature engineering
- pandas GroupBy operations
- Business KPI creation
- Customer analytics
- RFM segmentation
- Rule-based anomaly detection
- Exporting reporting datasets
- Data engineering project structuring

## How to Run

1. Open the notebook in Google Colab.
2. Upload `retail_black_friday_sales_100k.csv`.
3. Run all cells from top to bottom.
4. Download or review the exported CSV output files.

## Short Project Description

Built an end-to-end retail data engineering project using Python, pandas, Google Colab, and Kaggle data. Performed data ingestion, cleaning, transformation, KPI generation, customer analytics, RFM analysis, and suspicious transaction detection while creating analytics-ready reporting datasets.
