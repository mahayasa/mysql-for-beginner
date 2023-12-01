![MySQL for Beginners](./images/thumbnail.png)

# MySQL for Beginners : A Course
Welcome to the MySQL for Beginners repository! This guide is designed to help you get started with MySQL, a popular open-source relational database management system.


## Introduction

MySQL is a powerful and widely used relational database management system. It allows you to store, organize, and retrieve data efficiently. Whether you're a developer, a data analyst, or someone interested in databases, this guide will walk you through the basics of MySQL.

## Installation

To get started with MySQL, you need to install it on your machine. Follow the installation instructions for your operating system:
- [MySQL Installation Guide](https://dev.mysql.com/doc/mysql-installation-excerpt/8.0/en/)

## Connecting to MySQL

After installation, you can connect to MySQL using the command line or a graphical client. Learn how to connect and manage your MySQL server:
- [Connecting to MySQL](https://dev.mysql.com/doc/mysql-getting-started/en/)

## Basic Queries

Understand the fundamentals of SQL (Structured Query Language) and how to execute basic queries:
- [SQL Syntax](https://dev.mysql.com/doc/refman/8.0/en/sql-syntax.html)

## Creating a Database

Learn how to create a database to organize your data logically:
```sql
CREATE DATABASE mydatabase;

CREATE TABLE users (
    id INT PRIMARY KEY,
    username VARCHAR(50),
    email VARCHAR(100)
);
```

## Insert data into your tables using the INSERT statement:

```sql 
INSERT INTO users (id, username, email) VALUES (1, 'john_doe', 'john@example.com');
```

## Updating and Deleting Data

Learn how to update and delete records in your tables:

```sql
UPDATE users SET email = 'new_email@example.com' WHERE id = 1; 
DELETE FROM users WHERE id = 1;
```
## Course Part
|       |              Lesson Link              |                       Concepts Taught                       |                     Learning Goal                 |                             
| :---: | :------------------------------------: | :---------------------------------------------------------: | ----------------------------------------------------------- |
| 01 | [MySQL Tools](./01-tools-setup/README.md) | material setup  |  installed and configured XAMPP and PHPMyAdmin on your computer.| 
| 02 | [SQL Basic Concept](./02-sql-basic-concept/README.md) | primary and foreign key | Understanding primary and foreign keys is crucial for designing well-structured databases. | 
| 03 | [agregate Operation](./03-agregate-operation/README.md) | SQL COUNT,SUM,AVG,MAX,MIN | performing calculations and extracting insights from our database. | 
| 04 | [Join Statement](./04-join-statement/README.md) |  | | 
| 05 | [Other Operation](./05-other-operation/README.md) |  | | 
| 06 | [SQL Function](./06-sql-function/README.md) | | | 
| 07 | [SQL Procedure](./07-sql-procedure/README.md) | | | 
| 08 | [Final Project](./08-project-based/README.md) | | | 
