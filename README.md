# Advanced SQL Analytics Project

## Overview

This project demonstrates end-to-end data analysis using advanced SQL.  
The objective is to replicate real industry workflows, starting with structured Exploratory Data Analysis and progressing toward advanced analytical reporting using window functions, CTEs, subqueries, and performance logic.

All analysis is implemented purely in SQL.

---

## Objectives

- Explore and understand relational database structure  
- Perform systematic Exploratory Data Analysis  
- Conduct magnitude and ranking analysis  
- Apply advanced analytical techniques  
- Build consolidated reporting views  
- Answer real business questions using SQL  

---

## Dataset

The dataset simulates a transactional business environment (ecommerce-style schema) containing:

- Customers  
- Orders  
- Order Items  
- Products  
- Categories  

It includes transactional dates, quantities, pricing, and customer-level attributes.

---

## Project Roadmap

### Phase 1: Exploratory Data Analysis (EDA)

#### 1. Database Exploration
- Identify tables and relationships  
- Inspect primary and foreign keys  
- Understand table grain  
- Validate row counts  

#### 2. Dimension Exploration
- Unique counts per categorical column  
- Null value checks  
- Data consistency validation  

#### 3. Date Exploration
- Minimum and maximum transaction dates  
- Data coverage range  
- Missing period detection  

#### 4. Measure Exploration
- Total customers  
- Total orders  
- Total revenue  
- Average order value  

---

### Phase 2: Magnitude Analysis

Combine one dimension with one measure to understand scale and distribution.

Examples:
- Number of orders by product  
- Revenue by customer  
- Sales by category  
- Orders by region  

Techniques:
- GROUP BY  
- Aggregations  
- Proper join handling  

---

### Phase 3: Ranking Analysis

Identify top and bottom performers.

Examples:
- Top 10 customers by revenue  
- Top products by sales volume  
- Highest performing categories  

Techniques:
- ORDER BY  
- LIMIT  
- RANK()  
- DENSE_RANK()  
- ROW_NUMBER()  

---

### Phase 4: Advanced Analytical Techniques

#### 1. Change Over Time
- Monthly revenue trends  
- Month-over-month growth  
- Growth rate calculations  

Techniques:
- DATE_TRUNC  
- LAG()  
- Window functions  

#### 2. Cumulative Analysis
- Running revenue totals  
- Accumulated orders over time  

Technique:
- SUM() OVER (ORDER BY date)

#### 3. Performance Analysis
- Period-over-period comparison  
- Region comparison  
- Product performance evaluation  

Techniques:
- Window functions  
- CASE statements  

#### 4. Part-to-Whole Analysis
- Category contribution percentage  
- Customer revenue share  

Technique:
- value / SUM(value) OVER()

#### 5. Data Segmentation
- Customer segmentation by revenue  
- Frequency-based grouping  
- Value-based segmentation  

Techniques:
- CASE  
- Aggregation  
- Conditional grouping  

---

### Phase 5: Reporting Layer

Build a consolidated SQL view that:

- Answers multiple business questions  
- Combines trend analysis  
- Includes ranking and segmentation  
- Provides decision-ready metrics  

This simulates a production analytics view used by BI tools.

---

## SQL Concepts Used

- CTEs  
- Subqueries  
- Window Functions  
- Aggregations  
- Ranking Functions  
- Conditional Logic  
- Analytical Calculations  

---

## Key Business Questions Answered

- How has revenue evolved over time?  
- Who are the top contributing customers?  
- Which products drive the most revenue?  
- What percentage does each category contribute?  
- How does performance compare month over month?  

---

## Project Structure

ecommerce_project/
│
├── sql/
│ ├── 01_eda.sql
│ ├── 02_magnitude_analysis.sql
│ ├── 03_ranking.sql
│ ├── 04_advanced_analytics.sql
│ └── 05_reporting_view.sql
│
└── README.md

---

## What This Project Demonstrates

- Structured analytical thinking  
- Ability to move from raw data to insight  
- Production-level SQL organization  
- Business-oriented problem solving  
- Advanced window function proficiency  
