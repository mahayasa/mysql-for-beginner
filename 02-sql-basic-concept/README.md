# SQL Basics: Primary and Foreign Keys

Welcome to the SQL Basics GitHub notebook! This guide will introduce you to fundamental concepts in SQL, with a specific focus on primary and foreign keys.

## Introduction to SQL

SQL (Structured Query Language) is a domain-specific language used for managing and manipulating relational databases. It provides a standard way to interact with databases, including tasks such as querying data, updating records, and defining the structure of the database.

## Relational Databases

Relational databases organize data into tables, which consist of rows and columns. The relationships between tables are defined by keys, such as primary and foreign keys.

## Primary Key

A primary key is a unique identifier for a record in a table. It ensures that each row in a table can be uniquely identified. Every table should have a primary key, and it must contain unique values.

### Creating a Table with a Primary Key

```sql
CREATE TABLE employees (
    employee_id INT PRIMARY KEY,
    first_name VARCHAR(50),
    last_name VARCHAR(50),
    hire_date DATE
);
```
In this example, the employee_id column is designated as the primary key for the employees table.

## Foreign Key

A foreign key is a column or a set of columns in a table that refers to the primary key of another table. It establishes a link between the two tables and is used to enforce referential integrity.
```sql
CREATE TABLE orders (
    order_id INT PRIMARY KEY,
    product_id INT,
    customer_id INT,
    order_date DATE,
    FOREIGN KEY (product_id) REFERENCES products(product_id),
    FOREIGN KEY (customer_id) REFERENCES customers(customer_id)
);
```

In this example, the product_id and customer_id columns in the orders table are foreign keys that reference the primary keys in the products and customers tables, respectively.

## Referential Integrity
Referential integrity ensures that relationships between tables remain valid. It means that foreign key values must match an existing primary key in the referenced table.

## Examples
Let's look at some examples of using primary and foreign keys in SQL queries. For instance, retrieving all orders along with the customer details:

```sql
SELECT orders.order_id, orders.order_date, customers.customer_name
FROM orders
JOIN customers ON orders.customer_id = customers.customer_id;
```

## Conclusion

Understanding primary and foreign keys is crucial for designing well-structured databases. These keys establish relationships between tables, ensuring data integrity and consistency.
