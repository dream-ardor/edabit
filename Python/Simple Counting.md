## Simple Counting

Mubashir needs your help to count a specific digit in a list.

You have to create a function that takes two integers n and d and makes a list of squares of all numbers from 0...<= n and returns the count of the digits d in the list.
```python

Examples
count_digits(10, 1) ➞ 4
# Squared list from 0 to 10 = [0, 1, 4, 9, 16, 25, 36, 49, 64, 81, 100]
# Digit 1 appeared 4 times in the list.

count_digits(25, 2) ➞ 9 

count_digits(10, 1) ➞ 4
```
### 🐍 My Code
```python
count_digits = lambda n,d:str([x * x for x in range(n+1)]).count(str(d))
```
