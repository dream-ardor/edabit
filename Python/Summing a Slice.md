## Summing a Slice

Given a list and an integer n, return the sum of the first n numbers in the list.
```python
Examples
sum_first_n_nums([1, 3, 2], 2) ➞ 4

sum_first_n_nums([4, 2, 5, 7], 4) ➞ 18

sum_first_n_nums([3, 6, 2], 0) ➞ 0

Notes:
If n is larger than the length of the list, return the sum of the whole list.
```
### :snake: My Code
```python
sum_first_n_nums = lambda l, n:sum(l[:n])
```
