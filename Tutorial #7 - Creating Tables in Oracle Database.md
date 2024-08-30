# Study Guide: Tutorial #7 - Creating Tables in Oracle Database

## 1. Table Creation Syntax

The basic syntax for creating a table in Oracle database is:

```sql
CREATE TABLE table_name (
    column1_name datatype(size),
    column2_name datatype(size),
    ...
);
```

**Key Points:**
- Use the `CREATE TABLE` statement followed by the table name
- Define columns with their names and data types inside parentheses
- Separate column definitions with commas 

## 2. Data Types and Column Definitions

When creating a table, you need to specify the data type for each column. Common data types include:

- **VARCHAR2(size)**: For variable-length character strings
- **NUMBER(size)**: For numeric values
- **DATE**: For date and time values

**Example:**
```sql
CREATE TABLE employees (
    employee_name VARCHAR2(20),
    salary NUMBER(10),
    date_of_birth DATE
);
```

In this example:
- `employee_name` is defined as VARCHAR2 with a maximum length of 20 characters
- `salary` is defined as a NUMBER with up to 10 digits
- `date_of_birth` is defined as a DATE 

## 3. Understanding Column Size

The size specified in parentheses after the data type indicates:
- For VARCHAR2: Maximum number of characters allowed
- For NUMBER: Maximum number of digits allowed

**Note:** You can adjust the size based on your requirements. For example:
```sql
CREATE TABLE example (
    name VARCHAR2(10),
    gender CHAR(1),
    salary NUMBER(9),
    hire_date DATE
);
```

Here, `name` can store up to 10 characters, `gender` is a single character, and `salary` can have up to 9 digits. 

## 4. VARCHAR2 vs CHAR

While both VARCHAR2 and CHAR are used for storing character data, they differ in how they store data:

- **VARCHAR2**: Stores variable-length strings efficiently, using only the space needed for the actual data.
- **CHAR**: Stores fixed-length strings, always using the full specified length.

**Key Difference:** VARCHAR2 is generally more space-efficient for columns where the data length varies significantly. 

## Practice Exercises

1. Create a table named `students` with columns for student ID, name, age, and enrollment date.
2. Create a table for storing product information, including product name, price, and description.
3. Experiment with different data types and sizes to understand their impact on data storage.

Remember to refer to Oracle's official documentation for a comprehensive list of data types and their specific behaviors.
