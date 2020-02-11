## Factorial of a Positive Integer

Write a function that takes a positive integer and return its factorial.
```python
Examples
factorial(4) ➞ 24

factorial(0) ➞ 1

factorial(9) ➞ 362880
```
### :snake: My Code
```python
factorial = lambda Z: 1 if Z <= 1 else Z * factorial(Z-1)
```


