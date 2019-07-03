## Is the Number Symmetrical?
Create a function that takes a number as an argument and returns True or False depending on whether the number is symmetrical or not. A number is symmetrical when it is the same as its reverse.
```python
Examples
is_symmetrical(7227) ➞ True

is_symmetrical(12567) ➞ False

is_symmetrical(44444444) ➞ True

is_symmetrical(9939) ➞ False

is_symmetrical(1112111) ➞ True
```
### :stew:My Code
```python
is_symmetrical = lambda num: num == int((str(num)[::-1]));	
```
