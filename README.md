# CRUD Application

A simple Java Swing CRUD application built with NetBeans and MySQL.

## Features

- View all users in a table
- Create new user records
- Update existing user records
- Delete user records

## Tech Stack

- Java
- Swing UI
- MySQL
- JDBC
- NetBeans IDE
- XAMPP

## Requirements

- Java Development Kit (JDK)
- NetBeans IDE
- XAMPP
- MySQL JDBC driver

## Database Setup

1. Start MySQL from XAMPP.
2. Create a database named `java_crud_db`.
3. Create a `users` table with these columns:
   - `id`
   - `first_name`
   - `last_name`
   - `email`
   - `country`

Example SQL:

```sql
CREATE DATABASE java_crud_db;

USE java_crud_db;

CREATE TABLE users (
	id INT AUTO_INCREMENT PRIMARY KEY,
	first_name VARCHAR(100) NOT NULL,
	last_name VARCHAR(100) NOT NULL,
	email VARCHAR(150) NOT NULL,
	country VARCHAR(100) NOT NULL
);
```

## Configuration

Update the database settings in [src/javacrudapp/DBConnection.java] if needed:

- Database name: `java_crud_db`
- Username: `root`
- Password: empty by default for local XAMPP setup

## Run the Project

1. Open the project in NetBeans.
2. Make sure the MySQL server is running.
3. Build and run the project.

The application starts from [src/javacrudapp/JavaCrudApp.java].

## Acknowledgements

- This project was recreated as a learning exercise by following the YouTube tutorial:
  **"Java CRUD GUI Application with MySQL | Full Project Tutorial using NetBeans and XAMPP" by ELA TECH.**

# Learned

- Reinforced core Java concepts such as classes, objects, and method invocation
- How to implement CRUD (Create, Read, Update, Delete) operations using JDBC (Java Database Connectivity - allows Java applications to communicate with databases)
- Utilization of the Data Access Object (DAO) design pattern for database interactions
- The use of Apache NetBeans for efficient project organization (Note: the GUI builder for Swing)
- How to configure and manage databases using XAMPP and phpMyAdmin
