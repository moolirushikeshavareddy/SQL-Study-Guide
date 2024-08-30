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

3. **Execution Order: In a DELETE statement, the clauses are executed in this order:**
   - FROM clause
   - WHERE clause 

## 4. Example Usage

Consider a table named 'employees' with columns: employee_id, name, department.

To delete an employee with ID 100:

```sql
DELETE FROM employees
WHERE employee_id = 100;
```

This statement will remove the row where the employee_id is 100. 

## 5. Best Practices

[1. **Always use a WHERE clause**: Unless you intend to delete all rows, always include a WHERE clause to specify which rows to delete.
2. **Test your DELETE statements**: Before running a DELETE statement on a production database, test it on a small subset of data or a test environment.
3. **Use transactions**: Wrap your DELETE statements in transactions so you can rollback if necessary]: #

   - Always use a WHERE clause unless you intend to delete all rows.
   - Double-check your WHERE condition before executing the DELETE statement.
   - Consider using a SELECT statement with the same WHERE clause to preview which rows will be deleted.
   - Use transactions for complex delete operations to ensure data integrity.

## 6. Example

```sql
DELETE FROM employees
WHERE department_id = 10;
```

This statement will delete all employees from department 10.

## 7. Practice Questions

1. What is the primary purpose of the DELETE operation in SQL?
2. How does DELETE differ from TRUNCATE?
3. What happens if you omit the WHERE clause in a DELETE statement?
4. In what order are the clauses in a DELETE statement executed? 
5. Write a DELETE statement to remove all employees from the 'IT' department?
6. How would you delete the oldest employee from the table?
7. Write a DELETE statement that removes employees hired before 2010?

Remember, the DELETE operation is powerful and can significantly affect your data (or) permanently removes data from your table. Always double-check your WHERE conditions before executing a DELETE statement.
