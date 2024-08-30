# Study Guide: Tutorial #9 - Renaming Tables in Oracle SQL

## 1. Introduction to Rename Operation

The rename operation in Oracle SQL is used to change the name of an existing object in the database. 

## 2. Objects That Can Be Renamed

You can rename various database objects using the rename operation, including:
- Tables
- Views
- Synonyms
- Sequences 

## 3. Syntax for Renaming a Table

The basic syntax for renaming a table in Oracle SQL is:

```sql
RENAME old_table_name TO new_table_name;
```

**Key points:**
- Use the keyword `RENAME`
- Specify the current table name (`old_table_name`)
- Use the keyword `TO`
- Provide the desired new table name (`new_table_name`) 

## 4. Example of Renaming a Table

Let's say we want to rename a table called "my_table" to "student":

```sql
RENAME my_table TO student;
```

## 5. Executing the Rename Command

To execute the rename command, you can:
1. Select the entire SQL statement
2. Press Ctrl+Enter
3. Alternatively, click the execution button in your SQL development environment 

## 6. Important Considerations

- Ensure you have the necessary permissions to rename objects in the database
- Be cautious when renaming objects, as it may affect existing queries or applications that reference the old name
- It's a good practice to update any dependencies after renaming an object

## 7. Review Questions

1. What is the purpose of the rename operation in Oracle SQL?
2. List at least three types of database objects that can be renamed.
3. Write the SQL syntax to rename a table called "employees" to "staff".
4. What keyword is used between the old and new table names in the rename syntax?
5. Describe two ways to execute a rename command in your SQL environment.

By understanding and practicing these concepts, you'll be able to effectively rename tables and other objects in Oracle SQL.
