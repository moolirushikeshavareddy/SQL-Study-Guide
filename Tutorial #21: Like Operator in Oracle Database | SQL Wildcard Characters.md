# Study Guide: Tutorial #21: Like Operator in Oracle Database | SQL Wildcard Characters

## Overview of the LIKE Operator
The **LIKE operator** is used in SQL to search for a specified pattern in a column. It is commonly used with wildcard characters to enhance search capabilities.

### Wildcard Characters
- **Percentage Symbol (%)**: Represents zero or more characters.
- **Underscore (_) **: Represents a single character.

## Examples of Using the LIKE Operator
1. **Searching for First Names**:
   - To find records where the first name starts with 'S':
     ```sql
     SELECT * FROM employee WHERE first_name LIKE 'S%';
     ```
   - This query retrieves all employees whose first names begin with 'S' .

2. **Searching for Last Names**:
   - To find records where the last name ends with 'XYZ':
     ```sql
     SELECT * FROM employee WHERE last_name LIKE '%XYZ';
     ```
   - This retrieves all employees whose last names end with 'XYZ' .

3. **Searching for Specific Keywords**:
   - To find records where the first name contains 'SD' or 'ABCD':
     ```sql
     SELECT * FROM employee WHERE first_name LIKE '%SD%' OR first_name LIKE '%ABCD%';
     ```
   - This retrieves employees whose first names include either 'SD' or 'ABCD' .

## Practical Application
- The LIKE operator is a powerful tool for filtering records based on patterns. 
- It is essential to practice using this operator in different scenarios to gain proficiency .

## Key Points to Remember
- The LIKE operator is part of the comparison operators in SQL.
- Always use the percentage symbol (%) and the word LIKE when forming your queries .
- Experiment with different patterns to understand how the LIKE operator works in various contexts.

## Questions to Consider
- How would you modify a query to find all employees whose names contain a specific substring?
- What are the differences between using the percentage symbol and the underscore in your queries? 
