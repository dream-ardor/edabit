## SQL AND Operator

A supermarket is keeping the record of their customers in SQL Table. They have decided to give some discount to their regular customers. They need your help to filter out their regular customers.
```sql
SELECT ColumnName FROM Table
WHERE OneColumn<10000 AND SecondColumn>=50;
In this challenge, fill in the query in the Code tab to select the data from the Name column having Bill greater than or equal to 15000 AND number of Vists greater than or equal to 15 from the table customers (see Tests tab).

Original Table

Name	    Bill	 Visits
Mubashir	25000	 29
Joshua	  30000	 37
Adam     	50000	 10
Bob	      30000	 15
Charlotte	20000	 14
Dillon	  15000	 13
Eileen	  9000	 7

Expected Results

Name
Mubashir
Joshua
Bob
```
### My Code
```sql
query = "SELECT Name FROM customers Where Bill >= 15000 AND Visits >= 15"
```
