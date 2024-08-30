# Study Guide: Tutorial #13 - SQL DELETE Operation

## 1. Introduction to DELETE Operation

The DELETE operation is a part of the Data Manipulation Language (DML) in SQL. It is used to remove specific rows from a table in a database. 

## 2. Syntax of DELETE Statement

The basic syntax for the DELETE operation is:

```sql
DELETE FROM table_name
WHERE condition;
```

- `DELETE FROM` is a keyword
- `table_name` is the name of the table from which you want to delete records
- `WHERE condition` specifies which rows to delete 

## 3. Key Points to Remember

1. **Specificity**: DELETE allows you to remove specific rows based on the WHERE condition. 

2. **Comparison with TRUNCATE**:
   - DELETE removes specific rows; TRUNCATE removes all rows.
   - DELETE is slower as it deletes data row by row.
   - TRUNCATE is faster as it deletes all data at once.  

## 4. Example Usage

Consider a table named 'employees' with columns: employee_id, name, department.

To delete an employee with ID 100:

```sql
DELETE FROM employees
WHERE employee_id = 100;
```

This statement will remove the row where the employee_id is 100. 

## 5. Practice Exercises

1. Write a DELETE statement to remove all employees from the 'IT' department.
2. How would you delete the oldest employee from the table?
3. Write a DELETE statement that removes employees hired before 2010.

## 6. Best Practices

- Always use a WHERE clause unless you intend to delete all rows.
- Double-check your WHERE condition before executing the DELETE statement.
- Consider using a SELECT statement with the same WHERE clause to preview which rows will be deleted.
- Use transactions for complex delete operations to ensure data integrity.

Remember, the DELETE operation permanently removes data from your table. Always be cautious and verify your conditions before executing a DELETE statement.
