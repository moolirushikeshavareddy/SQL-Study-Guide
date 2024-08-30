# Study Guide: Tutorial #12 - Oracle SQL - Data Manipulation Language (DML)

## 1. Introduction to DML
Data Manipulation Language (DML) is a subset of SQL that deals with manipulating data within database tables. It includes three main operations:
- Insert
- Delete
- Update


## 2. INSERT Statement

### 2.1 Purpose
The INSERT statement is used to add new data into Oracle database tables. 

### 2.2 Syntax
There are two main syntaxes for the INSERT statement:

1. **INSERT with column names and values:**
   ```sql
   INSERT INTO table_name
   COLUMN(column1, column2, column3, ...)
   VALUES (value1, value2, value3, ...);
   ```
                                             **OR**
   ```sql
   INSERT INTO table_name
   VALUES (value1, value2, value3, ...);
   ```
   

3. **INSERT with values only (not covered in detail in the excerpts)**

### 2.3 Key Points to Remember
1. **Column Order:** The order of columns in the INSERT statement must match the order of values provided. 

2. **Complete Data:** You must provide values for all columns listed in the INSERT statement. If your table has 20 columns, you need to supply values for all 20 columns. 

3. **Data Types:** Ensure that the values you're inserting match the data types of the corresponding columns.

## 3. Example
Example1:
```sql
INSERT INTO employees
COLUMN(employee_id, employee_name, hire_date)
VALUES (101, 'John Doe', '2023-06-15');
```
Example2:
```sql
INSERT INTO employees
VALUES (101, 'John Doe', '2023-06-15');
```
This example inserts a new record into the 'employees' table with an ID, name, and hire date. 

## 4. Best Practices
- Always specify the column names in your INSERT statement to ensure data integrity.
- Use prepared statements or parameterized queries when inserting data from user input to prevent SQL injection.
- Consider using batch inserts for large amounts of data to improve performance.

## 5. Related Topics
- DELETE statement (for removing data)
- UPDATE statement (for modifying existing data)
- Data Definition Language (DDL) operations like TRUNCATE (which we covered in a previous session) 

Remember to practice these concepts hands-on in an Oracle SQL environment for better understanding and retention.
