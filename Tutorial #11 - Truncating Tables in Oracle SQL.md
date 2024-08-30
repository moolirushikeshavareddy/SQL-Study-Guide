# Study Guide: Tutorial #11 - Truncating Tables in Oracle SQL

## 1. Definition of TRUNCATE

The TRUNCATE SQL statement is used to remove all data from a table in one operation. It's a quick way to delete all rows from a table without deleting the table structure itself. 

## 2. Key Points about TRUNCATE

- **Purpose**: Removes all data from a table instantly
- **Speed**: Faster than DELETE for removing all rows
- **Scope**: Affects the entire table, cannot use WHERE clause
- **Permissions**: Only database owner and table owner can perform TRUNCATE 

## 3. TRUNCATE vs DELETE

Understanding the differences between TRUNCATE and DELETE is crucial:

| Feature | TRUNCATE | DELETE |
|---------|----------|--------|
| Speed | Fast (one shot) | Slower (row by row) |
| WHERE clause | Not allowed | Allowed |
| Granularity | Whole table | Can target specific rows |



## 4. When to Use TRUNCATE

- When you need to remove all data from a table quickly
- When you don't need to filter which rows to remove
- When you have the necessary permissions (database or table owner)

## 5. Syntax

```sql
TRUNCATE TABLE table_name;
```

## 6. Important Considerations

- ==TRUNCATE is a DDL (Data Definition Language) command==
- It cannot be rolled back (in most cases)
- It resets identity columns (if any) in the table
- It's faster than DELETE because it doesn't generate individual row delete logs

## 7. Practice Questions

1. What is the main purpose of the TRUNCATE statement in SQL?
2. How does TRUNCATE differ from DELETE in terms of speed and functionality?
3. Who can perform a TRUNCATE operation on a table?
4. Can you use a WHERE clause with TRUNCATE? Why or why not?
5. In what scenarios would you choose TRUNCATE over DELETE?

Remember to practice writing and executing TRUNCATE statements in a safe, non-production environment to fully understand their impact and behavior. 
