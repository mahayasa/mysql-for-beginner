# SQL Query Conditional Operation: WHERE, ORDER BY, GROUP BY, HAVING 

**Welcome to the SQL Query GitHub README!** In this guide, we will explore essential SQL clauses, including WHERE, ORDER BY, GROUP BY, and HAVING. These clauses allow you to filter, sort, group, and apply conditions to your SQL queries.

## WHERE Clause

The WHERE clause is used to filter records based on a specified condition.

```sql
SELECT columns
FROM table
WHERE condition;
```

## ORDER BY Clause

The ORDER BY clause is used to sort the result set based on one or more columns.

```sql
SELECT columns
FROM table
ORDER BY column1 [ASC | DESC], column2 [ASC | DESC], ...;
```

## GROUP BY Clause

The GROUP BY clause is used to group rows that have the same values in specified columns.

```sql
SELECT column1, column2, aggregate_function(column3)
FROM table
GROUP BY column1, column2;
```

## HAVING Clause

The HAVING clause is used to filter the results of a GROUP BY query based on specified conditions.

```sql
SELECT column1, aggregate_function(column2)
FROM table
GROUP BY column1
HAVING condition;
```


## Examples

Let's explore some practical examples of using these clauses:

### Example 1: WHERE Clause

```sql
SELECT product_name, price
FROM products
WHERE price > 50;
```

### Example 2: ORDER BY Clause

```sql
SELECT customer_name, order_date
FROM orders
ORDER BY order_date DESC;
```

### Example 3: GROUP BY and HAVING Clauses

```sql
SELECT department, AVG(salary) as avg_salary
FROM employees
GROUP BY department
HAVING AVG(salary) > 50000;
```

## Conclusion

Understanding the WHERE, ORDER BY, GROUP BY, and HAVING clauses is crucial for crafting precise and insightful SQL queries. These clauses allow you to filter, sort, group, and apply conditions to your data effectively.

## Resources

- [W3Schools SQL WHERE Clause](https://www.w3schools.com/sql/sql_where.asp)
- [W3Schools SQL ORDER BY Clause](https://www.w3schools.com/sql/sql_orderby.asp)
- [W3Schools SQL GROUP BY Clause](https://www.w3schools.com/sql/sql_groupby.asp)
- [W3Schools SQL HAVING Clause](https://www.w3schools.com/sql/sql_having.asp)

Feel free to explore and practice with these clauses in your SQL queries. Happy querying!
