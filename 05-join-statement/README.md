# SQL JOIN Operations

**Welcome to the SQL JOIN Operations GitHub README!** In this guide, we will explore different types of JOIN operations in SQL, including INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL JOIN.

## INNER JOIN

The INNER JOIN keyword selects records that have matching values in both tables.

```sql
SELECT columns
FROM table1
INNER JOIN table2 ON table1.column_name = table2.column_name;
```

## LEFT JOIN

The LEFT JOIN keyword returns all records from the left table (table1) and the matched records from the right table (table2). The result is NULL from the right side if there is no match.

```sql
SELECT columns
FROM table1
LEFT JOIN table2 ON table1.column_name = table2.column_name;
```

## RIGHT JOIN

The RIGHT JOIN keyword returns all records from the right table (table2) and the matched records from the left table (table1). The result is NULL from the left side when there is no match.

```sql
SELECT columns
FROM table1
RIGHT JOIN table2 ON table1.column_name = table2.column_name;
```

## FULL JOIN

The FULL JOIN keyword returns all records when there is a match in either the left (table1) or the right (table2) table records.

```sql
SELECT columns
FROM table1
FULL JOIN table2 ON table1.column_name = table2.column_name;
```

## Combining Multiple JOINs

You can combine multiple JOIN operations in a single query.

```sql
SELECT columns
FROM table1
INNER JOIN table2 ON table1.column_name = table2.column_name
LEFT JOIN table3 ON table2.column_name = table3.column_name;
```

## Examples

Let's explore some practical examples of using these JOIN operations:

### Example 1: INNER JOIN

```sql
SELECT employees.employee_id, employees.first_name, departments.department_name
FROM employees
INNER JOIN departments ON employees.department_id = departments.department_id;
```

### Example 2: LEFT JOIN

```sql
SELECT customers.customer_id, orders.order_id
FROM customers
LEFT JOIN orders ON customers.customer_id = orders.customer_id;
```

## Conclusion

JOIN operations are fundamental for combining data from multiple tables in SQL. Understanding the differences between INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL JOIN is crucial for writing effective queries.

## Resources

- [W3Schools SQL JOIN Tutorial](https://www.w3schools.com/sql/sql_join.asp)
- [MySQL Documentation - JOIN Clause](https://dev.mysql.com/doc/refman/8.0/en/join.html)

Feel free to explore and practice with these JOIN operations in SQL. Happy querying!
