# Study Guide: Tutorial #17 - How Oracle SQL Query Works Internally

## 1. Introduction
This study guide covers the internal workings of a basic SQL SELECT statement in Oracle. We'll focus on how the query retrieves data from a table and how it determines which rows to select.

## 2. Basic SQL SELECT Statement
Let's start with a simple example:
```sql
SELECT * FROM employee WHERE employee_id = 100;
```
This query selects all columns from the employee table where the employee_id is 100. 

## 3. Query Execution Process

### 3.1 Initial Pointer Placement
When the query is triggered, Oracle places a pointer at the beginning of the table. 

### 3.2 Identifying Columns in WHERE Clause
The query engine identifies how many columns are mentioned in the WHERE clause. In our example, it's just one column: employee_id. 

### 3.3 Row Evaluation
For each row, Oracle:
1. Reads the value in the employee_id column
2. Compares it with the condition in the WHERE clause (employee_id = 100)
3. Marks the row as either matching or not matching the condition 

### 3.4 Condition Evaluation
Oracle internally evaluates the WHERE condition:
- If the left-hand side value (employee_id) equals the right-hand side value (100), the row is marked as a match.
- If not equal, the row is not selected. 

### 3.5 Row Selection
Only the rows that match the condition are selected and included in the result set. 

## 4. Key Points to Remember
- The query engine starts at the beginning of the table.
- It evaluates each row individually against the WHERE clause.
- The process continues until all rows have been checked.
- Only rows meeting the condition are returned in the result set.

## 5. Practice Exercise
Try to mentally walk through the execution process for the following query:
```sql
SELECT * FROM employee WHERE salary > 50000;
```
Think about how Oracle would evaluate each row and decide which ones to include in the result.

By understanding this internal process, you'll be better equipped to write efficient queries and troubleshoot performance issues in Oracle SQL.
