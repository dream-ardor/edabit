## Squares and Cubes

Create a function that takes a list of two numbers and checks if the square root of the first number is equal to the cube root of the second number.
```python
Examples
check_square_and_cube([4, 8]) ➞ True

check_square_and_cube([16, 48]) ➞ False

check_square_and_cube([9, 27]) ➞ True
```
### 🐍 My Code
```python
check_square_and_cube = lambda a:a[0] ** 1.5 == a[1]
```
