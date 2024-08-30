# Study Guide: Tutorial #14 - Updating Rows in Oracle SQL

## 1. Introduction to UPDATE Operation

The UPDATE operation is a crucial part of Data Manipulation Language (DML) in Oracle SQL. It allows you to modify existing data in database tables. 

## 2. Purpose of UPDATE Statement

The primary purpose of the SQL UPDATE statement is to update existing records in a table within an Oracle database. 

## 3. Syntax of UPDATE Statement

The basic syntax for the UPDATE statement is:

```sql
UPDATE table_name
SET column1 = value1, column2 = value2, ...
WHERE condition;
```

**Key components:**
- `UPDATE`: Keyword to initiate the update operation
- `table_name`: The name of the table you want to update
- `SET`: Keyword followed by the columns and their new values
- `WHERE`: Optional clause to specify which rows to update 

## 4. Example of UPDATE Statement

Let's consider an example where we want to update all employees' salaries to 300:

```sql
UPDATE employees
SET salary = 300;
```

This statement will update the `salary` column for all rows in the `employees` table to 300. 

## 5. Important Points to Remember

- Without a WHERE clause, the UPDATE statement will affect all rows in the table.
- You can update multiple columns in a single UPDATE statement.
- Always use the WHERE clause carefully to avoid unintended updates.
- It's a good practice to test your UPDATE statements on a small subset of data before applying them to the entire table.

## 6. Practice Exercises

1. Write an UPDATE statement to change the salary of an employee with a specific employee ID.
2. Update the hire date of all employees who joined before 2010 to '01-JAN-2010'.
3. Increase the salary by 10% for all employees in a specific department.

Remember to always backup your data before performing UPDATE operations, especially when dealing with large datasets or important information.
