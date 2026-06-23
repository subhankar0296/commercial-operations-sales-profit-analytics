# Commercial Operations Sales & Profit Analytics Dashboard

## Overview

This project demonstrates an end-to-end Business Intelligence solution built using SQL Server and Power BI to analyze commercial sales performance, profitability, product contribution, and regional trends.

The objective was to transform raw transactional data into actionable business insights by leveraging SQL for data preparation and analysis, followed by Power BI for data modeling, KPI development, and interactive dashboard creation.

---

## Business Problem

Businesses need a centralized view of sales and profitability to identify growth opportunities, monitor operational performance, and make data-driven decisions.

This project addresses key business questions:

* Which states generate the highest sales and profit?
* Which product categories contribute the most to profitability?
* How are sales and profit margins trending over time?
* Which markets drive overall business performance?
* What are the key drivers of profitability?

---

## Tools & Technologies

### SQL Server

* Data Exploration
* Data Cleaning
* Joins
* Aggregations
* Window Functions
* Stored Procedures
* User Defined Functions (UDFs)
* Table-Valued Functions (TVFs)
* Transaction Control

### Power BI

* Data Modeling
* Power Query
* DAX Measures
* KPI Development
* Interactive Dashboards
* Data Visualization

---

## Database Design

The project follows a Star Schema model consisting of:

### Fact Table

* **`dbo.Fact`**: Tracks core quantitative metrics including `Sales`, `COGS`, `Total_Expenses`, `Profit`, `Marketing`, `Inventory`, and `Date`.

### Dimension Tables
* **`dbo.Product`**: Contains item attributes including `ProductID`, `Product`, `Product_Type`, and operational segment `Type`.
* **`dbo.Location`**: Houses geographical attributes including `Area_Code` and `State`.

---

## SQL Analysis

Key SQL operations performed include:

* Sales and Profit Analysis
* Product-wise Performance Evaluation
* State-wise Revenue Analysis
* Profitability Calculations
* Ranking Products using Window Functions
* Hierarchical Aggregations using ROLLUP
* Stored Procedure Development
* Scalar and Table-Valued Functions
* Transaction Management using BEGIN TRANSACTION, COMMIT, and ROLLBACK

### Advanced SQL Concepts Used

* DENSE_RANK()
* CASE WHEN
* GROUP BY ROLLUP
* Stored Procedures
* Scalar UDFs
* Inline Table-Valued Functions
* Transactions

---

## Power BI Dashboard

The Power BI Executive Dashboard provides a comprehensive view of business performance through:

### Key Performance Indicators

* Total Sales
* Total COGS
* Total Expenses
* Net Profit
* Net Profit Margin %

### Visualizations

* Regional Sales vs Profit Analysis
* Sales by Market Distribution
* Product Profitability Ledger
* Revenue & Profit Growth Trends
* Interactive Filters for Date, State, and Product

---

## Key Insights

* Generated **$819.81K** in Total Sales.
* Achieved **$231.48K** Net Profit.
* Maintained a **28.24% Profit Margin**.
* California emerged as the highest-performing state.
* West and Central markets contributed the largest share of revenue.
* Coffee delivered the highest profit margin among all product categories.
* Revenue remained stable while profitability improved over time.

---

## Dashboard Preview

<img width="850" height="474" alt="image" src="https://github.com/user-attachments/assets/7b235f60-40a8-4914-a2b7-3031b8ac7472" />

---

## Project Workflow

1. Data Collection
2. Data Cleaning & Validation
3. SQL Data Analysis
4. Data Modeling
5. DAX Measure Creation
6. Dashboard Development
7. Business Insight Generation

---

## Repository Structure

```text
├── Data/
│   └── Fact.csv
    └── Location.csv
    └── Product.csv
├── SQL/
│   └── commercial-operations-sales-profit-analytics.sql
│
├── PowerBI/
│   └── Commercial Operations Sales & Profit Margin Executive Dashboard.pbix
│
├── Images/
│   └── dashboard_preview.png
│
└── README.md
```

---

## Business Value

This solution enables stakeholders to monitor financial performance, evaluate product profitability, analyze regional trends, and support strategic decision-making through an interactive business intelligence dashboard.

---

## Author

**Subhankar Mondal**

SQL | Power BI | Python | Data Analytics | Business Intelligence
