## Recursion: Array Sum
Write a function that recursively finds the sum of a list.
```python
Examples
sum_recursively([1, 2, 3, 4]) ➞ 10

sum_recursively([1, 2]) ➞ 3

sum_recursively([1]) ➞ 1

sum_recursively([]) ➞ 0
```
### My Code
```python
def sum_recursively(lst):
  if len(lst) == 0:
    return 0
  else:
    return lst[0] + sum_recursively(lst[1:])	
```
