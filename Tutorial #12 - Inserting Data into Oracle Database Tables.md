# Study Guide: Tutorial #12 - Inserting Data into Oracle Database Tables

## 1. INSERT Statement Basics

The INSERT statement is used to add new data into Oracle database tables. 

## 2. Syntax

There are two main syntaxes for the INSERT statement:

### 2.1 Syntax with Column Names

```sql
INSERT INTO table_name (column1, column2, column3, ...)
VALUES (value1, value2, value3, ...);
```

### 2.2 Syntax without Column Names

```sql
INSERT INTO table_name
VALUES (value1, value2, value3, ...);
```

## 3. Key Points to Remember

1. **Column Order**: When using the syntax with column names, ensure that the order of values matches the order of columns specified. 

2. **Complete Data**: You must provide values for all columns in the table, or at least for all columns that don't have default values or allow NULL. 

3. **Data Types**: Ensure that the values you're inserting match the data types of the corresponding columns.

4. **Quotes**: Use single quotes for string and date values.

## 4. Example
Example1:
```sql
INSERT INTO employees (employee_id, employee_name, hire_date)
VALUES (101, 'John Doe', to_date('3072024' 'ddmmyyyy');
```
Example2:
```sql
INSERT INTO employees
VALUES (101, 'John Doe', to_date('30/7/2024' 'dd/mm/yyyy');
```
This example inserts a new record into the 'employees' table with an ID, name, and hire date. 

## 4. To_date function:
**Example:**
 ```sql
to_date('30/7/2024' 'dd/mm/yyyy');
to_date('30-7-2024' 'dd-mm-yyyy');
to_date('3072024' 'ddmmyyyy');
to_date('30724' 'ddmmyy');

				OR

'30June2024'
'30June24'
```

**NOTE:**
- '30062024', it is an error don't use 06 use July
- zero(0) is the value in the database whereas null is empty in database

## 5. Best Practices
- Always specify the column names in your INSERT statement to ensure data integrity.
- Use prepared statements or parameterized queries when inserting data from user input to prevent SQL injection.
- Consider using batch inserts for large amounts of data to improve performance.

## 5. Practice Exercises

1. Create a simple table with at least 3 columns of different data types.
2. Write an INSERT statement to add a row to your table using the syntax with column names.
3. Write another INSERT statement to add a row using the syntax without column names.
4. Try inserting data with mismatched column order and observe the error.
5. Attempt to insert data omitting a required column and note the error message.

Remember: Always double-check your data and syntax before executing INSERT statements to maintain data integrity in your database.
