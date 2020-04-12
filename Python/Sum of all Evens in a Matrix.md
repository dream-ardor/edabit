## Sum of all Evens in a Matrix

Create a function that returns the sum of all even elements in a 2D matrix.
```python
Examples
sum_of_evens([
  [1, 0, 2],
  [5, 5, 7],
  [9, 4, 3]
]) ➞ 6

// 2 + 4 = 6

sum_of_evens([
  [1, 1],
  [1, 1]
]) ➞ 0

sum_of_evens([
  [42, 9],
  [16, 8]
]) ➞ 66

sum_of_evens([
  [],
  [],
  []
]) ➞ 0
```
### :snake: My Code
```python
sum_of_evens = lambda l:sum(a for b in l for a in b if not a % 2)
```
