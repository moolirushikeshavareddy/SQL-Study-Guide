# Study Guide: Tutorial #6 - Types (Classification) of SQL Statements in Oracle Database

## Introduction
In this tutorial, we'll explore the classification of SQL statements in Oracle databases. This knowledge is crucial for understanding how to interact with and manage Oracle databases effectively.

## SQL Statement Classifications

SQL statements in Oracle are divided into five main categories:

1. **Data Definition Language (DDL)**
2. **Data Manipulation Language (DML)**
3. **Data Control Language (DCL)**
4. **Transaction Control Language (TCL)**
5. **Data Query Language (DQL)** or Data Retrieval Language (DRL)



Let's examine each category in detail:

### 1. Data Definition Language (DDL)

DDL statements are used to define and modify the structure of database objects. Common DDL operations include:

- CREATE: Used to create new database objects
- ALTER: Used to modify existing database objects
- RENAME: Used to change the name of an existing object
- DROP: Used to remove database objects
- TRUNCATE: Used to clear the database objects



### 2. Data Manipulation Language (DML)

DML statements are used to manipulate data within database objects. Key DML operations include:

- INSERT: Used to add new data into a table
- UPDATE: Used to modify existing data in a table
- DELETE: Used to remove data from a table

### 3. Data Control Language (DCL)

DCL statements are used to control access to data within the database. Common DCL operations include:

- GRANT: Used to give specific privileges to users
- REVOKE: Used to take away privileges from users

### 4. Transaction Control Language (TCL)

TCL statements are used to manage the changes made by DML statements. Key TCL operations include:

- COMMIT: Used to save the changes
- ROLLBACK: Used to undo the changes
- SAVEPOINT: Used to create points within groups of transactions in which to ROLLBACK

### 5. Data Query Language (DQL) or Data Retrieval Language (DRL)

DQL statements are used to retrieve data from the database. The primary DQL operation is:

- SELECT: Used to retrieve data from one or more tables

## Key Points to Remember

- Understanding these classifications helps in organizing and managing SQL operations effectively.
- Each category serves a specific purpose in database management and manipulation.
- Proper use of these statements ensures data integrity, security, and efficient data retrieval.

## Practice Questions

1. What are the five main classifications of SQL statements in Oracle?
2. Which category does the CREATE statement belong to?
3. What is the primary purpose of DML statements?
4. How does a GRANT statement differ from a REVOKE statement?
5. What is the main operation in the DQL category?

By mastering these classifications, you'll have a solid foundation for working with Oracle databases and writing effective SQL queries. 
