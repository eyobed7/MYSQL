# MYSQL
### Installing MySQL

Installing on Windows
Download MySQL
Download MySQL installer from https://dev.mysql.com/downloads/installer/ and execute it. On this page you can select the version you would like to install. You can choose the web installer or the offline installer.
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture1.PNG)

## Install MySQL
Follow the below steps to install MySQL on Windows
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture2.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture3.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture4.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture5.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture6.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture7.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture8.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture9.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture10.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture11.PNG)
![capture](https://github.com/eyobed7/MYSQL/blob/main/Capture12.PNG)

# SQL CRUD Operations: Create, Read, Update, Delete

## 📘 Objective

The goal of this concept is to develop a solid understanding of **CRUD** (Create, Read, Update, Delete) operations—core tasks used for managing data in a database using **SQL**. By mastering these operations, you'll be equipped to effectively manipulate data in relational databases.

---

## 📚 Concept Overview

### 🔑 Topics Covered

- **DDL (Data Definition Language)**
- **DML (Data Manipulation Language)**
- **CRUD Operations in SQL**

---

## 🎯 Learning Objectives

- Understand the difference between **Data Definition** and **Data Manipulation** languages in SQL.
- Learn how to **create**, **read**, **update**, and **delete** data from a database.
- Practice CRUD operations using SQL commands.

---

## 🏗️ DDL (Data Definition Language)

**DDL statements** define and manage the structure of a database. Common commands include:

- `CREATE TABLE`: Create a new table.

  ```sql
  CREATE TABLE Customers (
      CustomerID INT PRIMARY KEY,
      Name VARCHAR(50),
      Email VARCHAR(100)
  );
  ```
**ALTER TABLE:** Modify an existing table.

```sql
ALTER TABLE Customers ADD Address VARCHAR(200);
```

**DROP TABLE:** Delete a table and its data.

```sql
DROP TABLE Customers;
```
**EXAMPLES**

```sql
  CREATE TABLE Students (
    StudentID INT PRIMARY KEY,
    FirstName VARCHAR(50) NOT NULL,
    LastName VARCHAR(50) NOT NULL,
    Email VARCHAR(100) UNIQUE,
    EnrollmentDate DATE
);

```
## 🛠️ DML (Data Manipulation Language)

DML statements manipulate data within tables.

**INSERT:** Add new records.

```sql
INSERT INTO Customers (Name, Email)
VALUES ('John Doe', 'john@example.com');
```
**UPDATE:** Modify existing records.

```sql
UPDATE Customers
SET Email = 'newemail@example.com'
WHERE CustomerID = 1;
```
**DELETE:** Remove records.

```sql
DELETE FROM Customers
WHERE CustomerID = 1;
```
---

Create a new table:

Create a new table called “Orders” with columns for OrderID (primary key), CustomerID (foreign key referencing the Students table), OrderDate, and Total.
Insert data into the Orders table:

Insert at least three new orders for different customers.
Read data from the Orders table:

Retrieve all orders placed on a specific date.
Retrieve orders for a specific customer, including the customer’s name and email from the Students table (using a JOIN).
Update data in the Orders table:

Update the Total column for a specific order.
Delete data from the Orders table:

Delete an order with a specific OrderID.

Additional Resources
[Crud](https://milnepublishing.geneseo.edu/themissinglink/chapter/chapter-41-mysql-crud-action/)
[Crud operation](https://retool.com/blog/crud-operations-sql)
