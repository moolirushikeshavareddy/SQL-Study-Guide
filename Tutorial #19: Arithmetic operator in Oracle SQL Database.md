# Study Guide: Tutorial #19: Arithmetic operator in Oracle SQL Database

## Overview
In this session, we will cover the **arithmetic operations** available in the Oracle database. Understanding these operations is crucial for performing calculations and data manipulation effectively.

## Arithmetic Operators
Oracle supports the following arithmetic operators:

- **Addition (+)**: Used to add two numbers.
- **Subtraction (-)**: Used to subtract one number from another.
- **Multiplication (*)**: Used to multiply two numbers.
- **Division (/)**: Used to divide one number by another.

These operators can be used in SQL queries to perform calculations on data from tables.

## Practical Application
### Example Query
To illustrate the use of arithmetic operators, consider the following SQL query that retrieves data from an employee table:

```sql
SELECT employee_id, salary, salary + 1000 AS new_salary
FROM employees;
```
In this example, we are adding 1000 to each employee's salary.

### Performing Operations
- **Addition Example**: 
  - If an employee's salary is 5000, the query will return a new salary of 6000.
  
- **Subtraction Example**:
  - To reduce a salary by a certain amount:
    ```sql
    SELECT employee_id, salary - 500 AS reduced_salary
    FROM employees;
    ```

- **Multiplication Example**:
  - To calculate a bonus:
    ```sql
    SELECT employee_id, salary * 1.10 AS bonus_salary
    FROM employees;
    ```
  
- **Division Example**:
  - To find the average salary:
    ```sql
    SELECT AVG(salary) AS average_salary
    FROM employees;
    ```

## Important Notes
- Ensure that the data types of the operands are compatible for the operations.
- Be cautious with division; dividing by zero will result in an error.

## Summary
Understanding and using arithmetic operators effectively can enhance your ability to manipulate and analyze data in Oracle databases. Practice these operations with real data to solidify your understanding.
