 # Study Guide: Tutorial #20: Comparison operator in Oracle SQL Database

## Overview
In this session, we explored **Comparison Operators** used in Oracle SQL, which are essential for querying and filtering data in databases.

## Key Comparison Operators
Here are the primary comparison operators you will use:

- **Equal to**: `=`
- **Not equal to**: `!=` or `<>`
- **Greater than**: `>`
- **Less than**: `<`
- **Greater than or equal to**: `>=`
- **Less than or equal to**: `<=`

These operators allow you to compare values in your SQL queries effectively .

## Example Queries
To illustrate how to use these operators, here are some example queries:

1. **Selecting records with a specific condition**:
   - To find records from the `employee` table where the salary is equal to 6000:
     ```sql
     SELECT * FROM employee WHERE salary = 6000;
     ```
   - This query will return all rows where the salary matches the specified value .

2. **Using Not Equal To**:
   - To find records where the salary is not equal to 6000:
     ```sql
     SELECT * FROM employee WHERE salary != 6000;
     ```

## Practice Assignment
To reinforce your understanding, try the following exercises:
- Write a query to find all employees with a salary greater than 5000.
- Write a query to find all employees whose first name is not 'John'.

## Conclusion
Understanding comparison operators is crucial for effective data retrieval in SQL. Practice using these operators in various queries to become more proficient in Oracle SQL .
