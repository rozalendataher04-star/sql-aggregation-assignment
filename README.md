# SQL Aggregation Functions Assignment

Route assignment on SQL aggregation functions, `GROUP BY` and `HAVING`.
It contains 20 queries (basic, intermediate, advanced) written in MySQL.

## Dataset

`Orders.csv` has 500 rows and 6 columns:

| Column | Description |
|---|---|
| OrderID | Unique order number |
| CustomerID | Customer code (30 customers) |
| ProductID | Product code (10 products) |
| Region | East, North, South or West |
| OrderDate | Order date (2023-01-01 to 2023-06-30) |
| Sales | Order value (50 to 5000) |

## Mapping from the assignment wording

The PDF asks about students, courses, departments and grades. This dataset is
sales data, so the terms were mapped as follows:

| Assignment term | Column used |
|---|---|
| Student | CustomerID |
| Course | ProductID |
| Department | Region |
| Grade | Sales |

## Adapted thresholds

Thresholds in some questions were changed to fit the Sales scale:

| Question | Original | Used |
|---|---|---|
| Q11 | average > 75 | average > 800 |
| Q12 | more than 3 courses | more than 8 products |
| Q13 | average < 65 | average < 800 |
| Q14 | max = 100 | max = 5000 |
| Q15 | at least 20 students | at least 25 customers |
| Q16 | average > 80 | average > 800 |

Q20 is a duplicate of Q19 in the original PDF.

## Files

| File | Description |
|---|---|
| `SQL_Aggregation_Assignment.sql` | All 20 queries |
| `Orders.csv` | The dataset |
| `screenshots/` | Result of each query |

## How to run

1. Create the database: `CREATE DATABASE sql_practice;`
2. Import `Orders.csv` into a table named `Orders`
   (MySQL Workbench: Table Data Import Wizard).
3. Open `SQL_Aggregation_Assignment.sql` and run the queries.

## Tools

- MySQL Workbench
- MySQL
