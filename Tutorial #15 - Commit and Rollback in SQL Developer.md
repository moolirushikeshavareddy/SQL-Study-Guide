# Study Guide: Tutorial #15 - Commit and Rollback in SQL Developer

## 1. Commit

### Definition
Commit is an operation that saves changes made in a transaction to the database. 

### Key Points
- Commit is used when you want to save any transaction. 
- It permanently applies changes to the database.
- Think of it like saving a file in Windows - once you commit, the changes are stored. 

### Example
Imagine you're updating a customer's address in a database:
1. You make the change
2. You review the change
3. You commit the change - this saves it permanently

## 2. Rollback

### Definition
Rollback is an operation used to undo changes that haven't been committed yet. 

### Key Points
- Rollback is used when you want to undo recent changes.
- It can only be used **before** a commit operation. 
- Rollback will undo all changes made since the last commit. 

### Example
Think of it like using "Ctrl+Z" in a text editor:
1. You make some changes to a database table
2. You realize the changes are incorrect
3. You use rollback to undo those changes 

## 3. Important Considerations

1. **Timing**: Rollback must be done ==before== commit. Once changes are committed, they can't be rolled back.

2. **Scope**: Rollback undoes all changes since the last commit, not just the most recent one.

3. **Data Integrity**: Proper use of commit and rollback helps maintain data integrity in your database.

4. **Transaction Management**: These operations are crucial for managing transactions in SQL Developer.

## 4. Practice Exercise
Try this in SQL Developer:
1. Start a transaction
2. Update a record
3. Use SELECT to view the change
4. Use ROLLBACK
5. Use SELECT again to confirm the rollback
6. Update the record again
7. Use COMMIT
8. Try to ROLLBACK (notice it doesn't work after commit)

Remember: Understanding commit and rollback is crucial for effective database management and maintaining data integrity in SQL Developer.
