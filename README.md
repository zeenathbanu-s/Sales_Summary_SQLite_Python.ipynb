# Task 7: Sales Summary from SQLite Database

## Overview
This project uses SQL queries in Python to analyze sales data from a SQLite database. It calculates total quantity sold and revenue per product, displaying the results via print and a bar chart.

## Tools Used
- **Python** (sqlite3, pandas, matplotlib)
- **SQLite** (built-in with Python)

## Setup
1. **Install Dependencies**:
   - sqlite3 (built-in)
   - pandas
   - matplotlib

2. **Create SQLite Database**:
   - `sales_data.db` containing a `sales` table with `product`, `quantity`, `price`.

3. **SQL Query**:
   ```sql
   SELECT product, SUM(quantity) AS total_qty, SUM(quantity * price) AS revenue
   FROM sales
   GROUP BY product
4.Result: The result of the query will be displayed as a table and a bar chart:


