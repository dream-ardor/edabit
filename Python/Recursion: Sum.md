## Recursion: Sum
Write a function that recursively finds the sum of the first n natural numbers.
```python
Examples
sum_numbers(5) ➞ 15
// 1 + 2 + 3 + 4 + 5 = 15

sum_numbers(1) ➞ 1

sum_numbers(12) ➞ 78
```
### :microscope:My Code
```python
def sum_numbers(n):
	if n <= 1:
	  return n
	else:
	  return n + sum_numbers(n-1)
```
