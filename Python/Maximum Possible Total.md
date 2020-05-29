## Maximum Possible Total

Given a list of 10 numbers, return the maximum possible total made by summing just 5 of the 10 numbers.
```python
Examples
max_total([1, 1, 0, 1, 3, 10, 10, 10, 10, 1]) ➞ 43

max_total([0, 0, 0, 0, 0, 0, 0, 0, 0, 100]) ➞ 100

max_total([1, 2, 3, 4, 5, 6, 7, 8, 9, 10]) ➞ 40
```
### :snake: My Code
```python
def max_total(n):
 n.sort()
 return sum(n[-5:])

#alternate
max_total=lambda l:sum(sorted(l)[5:])
```
