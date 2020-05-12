## Number to Reversed Array

Create a function that takes a number and returns a list with the digits of the number in reverse order.
```python
Examples
reverse_list(1485979) ➞ [9, 7, 9, 5, 8, 4, 1]

reverse_list(623478) ➞ [8, 7, 4, 3, 2, 6]

reverse_list(12345) ➞ [5, 4, 3, 2, 1]
```
### :snake: My Code
```python
reverse_list = lambda n:[int(i) for i in str(n)][::-1]
```
