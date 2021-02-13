## How Many Digits?

Given an integer n. Your task is to find how many digits this integer contains without using str or len methods!
```python
Examples
sum_digits(100) ➞ 3

sum_digits(1000) ➞ 4

sum_digits(1) ➞ 1
```
### :snake: My Code
```python
sum_digits = lambda n:1 if n < 10 else 1 + sum_digits(n/10)
	
```
