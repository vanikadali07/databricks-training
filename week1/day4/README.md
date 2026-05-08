# Week 1 - Day 4

## Overview
This day focused on practicing SQL Window Functions and analytical queries using PostgreSQL. The exercises helped in understanding ranking functions, running totals, cumulative calculations, and advanced data analysis techniques.

## Objectives
- Learn SQL window functions
- Perform ranking and analytical operations
- Understand PARTITION BY and ORDER BY usage
- Analyze data using running totals and moving averages

## Topics Covered

### Window Functions
- ROW_NUMBER()
- RANK()
- DENSE_RANK()
- NTILE()

### Partitioning and Ranking
- Using PARTITION BY
- Ranking employees within departments
- Finding top-performing records

### Analytical Functions
- LAG()
- LEAD()
- Running totals
- Cumulative calculations

### Aggregate Analysis
- Moving averages
- Department-wise highest salaries
- Sales analysis using window functions

## Tools Used
- PostgreSQL
- DB Fiddle
- GitHub

## Work Completed
- Created employees, customers, and orders tables
- Inserted sample records into all tables
- Practiced 15 SQL window function queries
- Implemented ranking and analytical queries
- Updated schema.sql, queries.sql, and output.txt files

## Key Examples Practiced
- Ranking employees based on salary
- Finding top 3 highest-paid employees
- Calculating running totals of sales
- Calculating cumulative sales per employee
- Finding previous and next order amounts using LAG() and LEAD()
- Calculating moving averages for orders
- Finding first and latest orders for each customer

## Challenges Faced
- Understanding PARTITION BY behavior
- Writing nested queries with window functions
- Calculating moving averages correctly
- Understanding LAG() and LEAD() operations

## Key Learnings
- Window functions allow advanced data analysis without grouping rows
- PARTITION BY helps divide data into logical sections
- LAG() and LEAD() are useful for comparing sequential records
- Running totals and moving averages help analyze trends
- Window functions simplify complex analytical queries

## Conclusion
Day 4 improved understanding of SQL analytical functions and advanced querying techniques. It also strengthened problem-solving skills for handling real-world business and sales data scenarios.
