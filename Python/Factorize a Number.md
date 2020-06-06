## Factorize a Number

Create a function that takes a number as its argument and returns a list of all its factors.
```python
Examples
factorize(12) ➞ [1, 2, 3, 4, 6, 12]

factorize(4) ➞ [1, 2, 4]

factorize(17) ➞ [1, 17]
```
### :snake: My Code
```python
factorize = lambda n:[x for x in range(1,n+1) if n % x == 0]
```
