# Study Guide: Tutorial #18: Logical Operators in SQL

## Overview of Logical Operators
Logical operators are essential in SQL for filtering records based on multiple conditions. In Oracle databases, there are three primary logical operators:

1. **AND**: Returns true if both conditions are true.
2. **OR**: Returns true if at least one of the conditions is true.
3. **NOT**: Reverses the truth value of the condition.

These operators help in constructing complex queries to retrieve specific data from tables .

## Truth Tables
Understanding the truth tables for these operators is crucial. Here’s a brief overview:

### AND Operator
| A     | B     | A AND B |
|-------|-------|---------|
| True  | True  | True    |
| True  | False | False   |
| False | True  | False   |
| False | False | False   |

### OR Operator
| A     | B     | A OR B  |
|-------|-------|---------|
| True  | True  | True    |
| True  | False | True    |
| False | True  | True    |
| False | False | False   |

### NOT Operator
| A     | NOT A |
|-------|-------|
| True  | False |
| False | True  |

These tables illustrate how the logical operators function .

## Practical Examples
### Using Logical Operators in SQL Queries
Here are some examples of how to use these logical operators in SQL statements:

1. **Using AND**:
   To retrieve records from the employee table where the employee ID is 100 and the first name is Stephen:
   ```sql
   SELECT * FROM employee WHERE employee_id = 100 AND first_name = 'Stephen';
   ```
   This query ensures that both conditions must be met for a record to be returned .

2. **Using OR**:
   To find employees with either a salary of 9000 or a first name of Stephen:
   ```sql
   SELECT * FROM employee WHERE salary = 9000 OR first_name = 'Stephen';
   ```
   This query returns records that meet at least one of the conditions .

3. **Using NOT**:
   To exclude employees with a salary of 9000:
   ```sql
   SELECT * FROM employee WHERE NOT salary = 9000;
   ```

## Key Points to Remember
- **AND** requires all conditions to be true.
- **OR** requires at least one condition to be true.
- **NOT** negates the condition.

## Questions to Consider
- How do you combine multiple conditions using logical operators?
- What is the difference between using AND and OR in a query?
- Can you write a query that uses all three logical operators?

This study guide should help you understand and apply logical operators effectively in SQL. Happy studying!
