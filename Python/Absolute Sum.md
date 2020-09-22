## Absolute Sum

Take a list of integers (positive or negative or both) and return the sum of the absolute value of each element.
```python
Examples
get_abs_sum([2, -1, 4, 8, 10]) ➞ 25

get_abs_sum([-3, -4, -10, -2, -3]) ➞ 22

get_abs_sum([2, 4, 6, 8, 10]) ➞ 30

get_abs_sum([-1]) ➞ 1

Notes:
The term "absolute value" means to remove any negative sign in front of a number, and to think of all numbers as positive (or zero).
All the elements in the given array are intergers.
```
### :snake: My Code
```python
get_abs_sum = lambda l:sum(abs(a) for a in l)
```
