# SQL Sales Database Assignment

## 📌 Project Overview

This project contains SQL queries used to retrieve and filter information from a **Sales Database**.

The assignment focuses on basic SQL operations such as:

* `SELECT`
* `WHERE`
* `ORDER BY`
* `LIMIT`
* Retrieving all records using `*`

## 🗄️ Database

**Database Name:** `sales`

The database contains the following tables:

* `payments`
* `orders`
* `employees`
* `offices`
* `products`

## 📝 Assignment Questions

### Question 1: Retrieve Payment Information

Retrieve the `checkNumber`, `paymentDate`, and `amount` from the `payments` table.

```sql
SELECT checkNumber, paymentDate, amount
FROM payments;
```

### Question 2: Find Orders in Process

Retrieve orders whose status is **In Process** and sort them by `orderDate` in descending order.

```sql
SELECT orderDate, requiredDate, status
FROM orders
WHERE status = 'In Process'
ORDER BY orderDate DESC;
```

### Question 3: Find Sales Representatives

Retrieve the first name, last name, and email of employees whose job title is **Sales Rep**.

The results are sorted by `employeeNumber` in descending order.

```sql
SELECT firstName, lastName, email
FROM employees
WHERE jobTitle = 'Sales Rep'
ORDER BY employeeNumber DESC;
```

### Question 4: Retrieve Office Information

Retrieve all columns and all records from the `offices` table.

```sql
SELECT *
FROM offices;
```

### Question 5: Retrieve the Five Cheapest Products

Retrieve the product name and quantity in stock for the five products with the lowest `buyPrice`.

```sql
SELECT productName, quantityInStock
FROM products
ORDER BY buyPrice ASC
LIMIT 5;
```

## ▶️ How to Run the Queries

First, select the `sales` database:

```sql
USE sales;
```

Then run each query individually in **MySQL Workbench**.

## 🛠️ Tools Used

* MySQL
* MySQL Workbench
* SQL
* GitHub

## 🎯 Learning Objectives

Through this assignment, I practiced:

1. Selecting specific columns from a table.
2. Filtering records using `WHERE`.
3. Sorting results using `ORDER BY`.
4. Sorting in ascending and descending order.
5. Limiting query results using `LIMIT`.
6. Retrieving all table columns using `SELECT *`.

## 👤 Author

**Abdiaziz**

SQL Database Assignment
