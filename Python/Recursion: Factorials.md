## Recursion: Factorials

Write a function that calculates the factorial of a number recursively.
```python
Examples
factorial(5) ➞ 120

factorial(3) ➞ 6

factorial(1) ➞ 1

factorial(0) ➞ 1
```
### :snake: My Code
```python
def factorial(n):
  return 1 if n < 1 else n * factorial(n-1)
	
```
