## Even Index Elements in a List

Create a function that takes a list of integers and returns the sum of all the integers that have an even index, multiplied by the integer at the last index.

For example:
```
[2, 3, 4, 5] ➞ 30
(2 + 4) * 5 ➞ 30

[1, 4, 5, 6, 7, 2, 3] ➞ 48
(1 + 5 + 7 + 3) * 3 ➞ 48

Examples
even_last([]) ➞ 0

even_last([1, 3, 3, 1, 10]) ➞ 140

even_last([-11, 3, 3, 1, 10]) ➞ 20
```
### 🐍 My Code
```python
even_last = lambda l:sum(l[::2]) * l[-1] if l else 0
```
