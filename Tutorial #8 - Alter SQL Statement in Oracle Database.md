# Study Guide: Tutorial #8 - Alter SQL Statement in Oracle Database

## 1. Introduction to Alter Statement

The ALTER statement is a powerful SQL command used to modify the definition of existing database objects, primarily tables. It allows you to make changes to the structure of a table without having to drop and recreate it. 

## 2. Key Operations with Alter Statement

The ALTER statement can perform several operations on a table:

1. **Rename columns**
2. **Modify columns**
3. **Add new columns**
4. **Remove existing columns**



## 3. Syntax for Common Alter Operations

### 3.1 Adding a Column

```sql
ALTER TABLE table_name
ADD column_name datatype;
```



### 3.2 Modifying a Column

```sql
ALTER TABLE table_name
MODIFY column_name new_datatype;
```

### 3.3 Renaming a Column

```sql
ALTER TABLE table_name
RENAME COLUMN old_column_name TO new_column_name;
```

### 3.4 Removing a Column

```sql
ALTER TABLE table_name
DROP COLUMN column_name;
```

## 4. Important Points to Remember

- The ALTER statement is applicable to various database objects, not just tables.
- It's a safe way to make changes to table structure without losing data.
- Always backup your data before performing ALTER operations, especially when changing data types.
- Some operations might have restrictions based on the current state of the table (e.g., you can't drop a column that's part of a primary key without first removing the constraint).



## 5. Practice Exercises

1. Create a simple table and add a new column to it using ALTER.
2. Modify the data type of an existing column.
3. Rename a column in your table.
4. Remove a non-essential column from your table.

## 6. Review Questions

1. What is the primary purpose of the ALTER statement in SQL?
2. List four operations you can perform using the ALTER statement.
3. What precautions should you take before using ALTER on a production database?
4. Can you use ALTER to change the name of a table? If yes, how?

By mastering the ALTER statement, you'll be able to efficiently manage and modify your database structures, adapting them to changing requirements without disrupting your data.
