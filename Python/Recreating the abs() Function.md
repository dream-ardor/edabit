## Recreating the abs() Function

The abs() function returns the absolute value of a number. This means that it returns a number's positive value. You can think of it as the distance away from zero.

Create a function that recreates this functionality.
```python
Examples
absolute(-5) ➞ 5

absolute(-3.14) ➞ 3.14

absolute(250) ➞ 250

Notes:
Tests will only include valid numbers.
Don't use the abs() function directly, that would defeat the challenge's purpose!
```
### :snake: My Code
```python
absolute = lambda n:n if n >= 0 else n * -1

```
