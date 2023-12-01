# SQL Aggregate Functions: SUM, AVG, MIN, MAX, COUNT

**Welcome to the SQL Aggregate Functions GitHub README!** In this guide, we will delve into the usage of SQL aggregate functions, specifically `SUM`, `AVG`, `MIN`, `MAX`, and `COUNT`. These functions allow you to perform calculations on a set of values within a column.

## SUM Function

The `SUM` function is used to calculate the sum of values in a numeric column.

```sql
SELECT SUM(column_name) AS total_sum FROM table_name;
```

## AVG Function

The `AVG` function calculates the average of values in a numeric column.

```sql
SELECT AVG(column_name) AS total_sum FROM table_name;
```

## MIN Function

The `MIN` function retrieves the minimum value in a column.

```sql
SELECT MIN(column_name) AS total_sum FROM table_name;
```

## MAX Function

The `MAX` function retrieves the maximum value in a column.

```sql
SELECT MAX(column_name) AS total_sum FROM table_name;
```

## COUNT Function

The `COUNT` function counts the number of rows in a specified column.

```sql
SELECT COUNT(column_name) AS total_sum FROM table_name;
```

## Examples

Let's explore some practical examples of using these aggregate functions:

### Example 1: Calculate the Total Sales

```sql
SELECT SUM(sales_amount) AS total_sales FROM sales;
```

### Example 2: Find the Average Age

```sql
SELECT AVG(age) AS average_age FROM employees;
```

### Example 3: Identify the Highest Score

```sql
SELECT MAX(score) AS highest_score FROM exam_results;
```

## Conclusion

SQL aggregate functions are powerful tools for performing calculations and extracting insights from your database. Whether you need to find totals, averages, minimums, maximums, or count rows, these functions provide valuable capabilities.

## Resources

- [SQL Aggregate Functions - W3Schools](https://www.w3schools.com/sql/sql_count_avg_sum.asp)
- [MySQL Documentation - Aggregate Functions](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html)

Feel free to explore and practice with these aggregate functions in SQL. Happy querying!
