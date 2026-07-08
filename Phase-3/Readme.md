# SQL to PySpark Phase 3 – Final ETL & Pipeline

## Objective

This phase focuses on building a complete ETL (Extract, Transform, Load) pipeline using PySpark. The goal is to move beyond writing individual SQL queries and learn how data engineers ingest, clean, transform, and prepare data for reporting.

---

## ETL Workflow

### Extract

* Read `customers.csv` 
* Read `sales.csv`

### Transform

* Inspect datasets using `show()` and `printSchema()`
* Remove rows with missing `customer_id`
* Convert `total_amount` to `Double`
* Convert `quantity` to `Integer`
* Remove invalid records
* Join customer and sales datasets
* Perform aggregations and generate reports

### Load

* Display the transformed results
* Optionally save the final reporting table as a CSV file

---

## Datasets Used

The datasets are located in the `/samples` directory.

### customers.csv

| Column       |
| ------------ |
| customer_id  |
| first_name   |
| last_name    |
| email        |
| phone_number |
| address      |
| city         |
| state        |
| zip_code     |

### sales.csv

| Column       |
| ------------ |
| sale_id      |
| customer_id  |
| product_id   |
| sale_date    |
| quantity     |
| total_amount |

---

## Data Cleaning Steps

* Removed rows with missing `customer_id`
* Converted `total_amount` from String to Double
* Converted `quantity` from String to Integer
* Filtered records where:

  * `total_amount > 0`
  * `quantity > 0`

---

## Business Exercises Completed

### 1. Daily Sales

Calculated total sales amount for each sale date.

### 2. City-wise Revenue

Joined customer and sales data to calculate total revenue generated from each city.

### 3. Repeat Customers

Identified customers who placed more than two orders.

### 4. Highest Spending Customer in Each City

Calculated customer-wise spending within each city and ranked by total spend.

### 5. Final Reporting Table

Generated a consolidated report containing:

* Customer ID
* Customer Name
* City
* Total Spend
* Order Count

---

## Project Structure

```
SQL-to-PySpark-Phase3/
│
├── SQL/
│   └── phase3.sql
│
├── PySpark/
│   └── phase3.py
│
├── Screenshots/
│   ├── exercise1.png
│   ├── exercise2.png
│   ├── exercise3.png
│   ├── exercise4.png
│   ├── exercise5.png
│
└── README.md
```

---

## Technologies Used

* Apache Spark
* PySpark
* SQL
* Spark Playground

---

## SQL Concepts Practiced

* SELECT
* GROUP BY
* ORDER BY
* HAVING
* INNER JOIN
* Aggregate Functions (SUM, COUNT)

---

## PySpark Concepts Practiced

* Reading CSV files
* Data inspection
* Data cleaning with `dropna()`
* Type conversion using `cast()`
* Filtering records
* `groupBy()`
* `agg()`
* `sum()`
* `count()`
* `join()`
* `orderBy()`
* Building an ETL pipeline

---

## Learning Outcomes

After completing this phase, I learned how to:

* Build a complete ETL pipeline using PySpark.
* Read and inspect datasets from CSV files.
* Clean and transform data before analysis.
* Perform joins and aggregations using PySpark.
* Convert SQL queries into equivalent PySpark transformations.
* Generate business reports using grouped and aggregated data.
* Organize PySpark projects using a structured workflow.

---

## Repository Contents

* SQL queries for all business exercises
* PySpark ETL pipeline implementation
* Output screenshots
* Project documentation
