## SQL COUNT() Function

In SQL, the COUNT() function returns the number of rows that match a specified criterion. You can use this syntax:
```sql
SELECT COUNT(column_name)
FROM table_name
WHERE condition;
```
In this challenge, fill in the query in the Code tab to COUNT the total visitors from the Name column, having Bill greater than 10000 AND number of Visits less than 15 from the table Customers (see Tests tab).
### :snake: My Code
```sql
query = "SELECT COUNT(Name) FROM customers WHERE Bill > 10000 AND VISITS < 15"
```
