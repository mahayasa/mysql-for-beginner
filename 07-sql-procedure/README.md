![MySQL for Beginner](./images/thumbnail.png)

# MySQL for Beginner : A Course
Welcome to the MySQL for Beginners repository! This guide is designed to help you get started with MySQL, a popular open-source relational database management system.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Connecting to MySQL](#connecting-to-mysql)
- [Basic Queries](#basic-queries)
- [Creating a Database](#creating-a-database)
- [Creating Tables](#creating-tables)
- [Inserting Data](#inserting-data)
- [Querying Data](#querying-data)
- [Updating and Deleting Data](#updating-and-deleting-data)
- [Resources](#resources)

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
