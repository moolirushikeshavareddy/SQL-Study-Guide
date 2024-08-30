# Study Guide: Oracle Database Data Types

## 1. What are Data Types?

Data types are rules imposed on columns in a database to ensure data integrity and consistency. 

## 2. Importance of Data Types

- **Data Validation**: Ensures only appropriate data is entered into a column.
- **Data Consistency**: Maintains uniformity across the database.
- **Optimization**: Helps in efficient storage and retrieval of data.

## 3. Where We Use Data Types

Data types are used when defining the structure of database tables. They are applied to individual columns to specify what kind of data each column can contain. 

### Example:
- A "Date of Birth" column with a DATE data type will only accept valid date values (e.g., 01-02-2018).
- It will reject invalid inputs like characters or incorrect date formats.

## 4. Types of Data Types in Oracle Database

Oracle database supports various data types, which can be classified into six main categories: 

1. **Number**
2. **Character**
3. **Date**
4. **LOB (Large Object)**
5. **ROWID**
6. **BFILE**

### Special Mention: LONG Data Type

- Can hold up to 2 GB of data in a single column of a row.
- Supports both numbers and characters. 

## Key Points to Remember

1. ==Data types are crucial for maintaining data integrity in databases.==
2. **Always choose the appropriate data type for each column based on the kind of data it will store.**
3. *Understanding data types helps in designing efficient and reliable database structures.*

By mastering these concepts, you'll be better equipped to work with Oracle databases and ensure data is stored and managed effectively.
