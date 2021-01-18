## SQL ORDER BY Keyword

Once you've learned how to SELECT everything from a table in SQL, you can sort your results in ascending or descending order. By default, SQL will always sort the results in ascending order. For Example :
```sql
SELECT * FROM Table
ORDER BY ColumnName
is same as :

SELECT * FROM Table
ORDER BY ColumnName ASC
You can sort the results in descending order by using this syntax :

SELECT * FROM Table
ORDER BY ColumnName DESC
```
In this challenge, fill in the query in the Code tab to select All Data from the table Customers sorted by Visits column in Ascending Order (see Tests tab).
### My Code
```sql
query = "SELECT * FROM customers ORDER BY Visits ASC"
```
