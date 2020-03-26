## Does a Number Exist?

Create a function which validates whether a given number exists, and could represent a real life quantity.

Inputs will be given as a string.
```python
Examples
valid_str_number('3.2') ➞ True

valid_str_number('324') ➞ True

valid_str_number('54..4') ➞ False

valid_str_number('number') ➞ False
```
### :snake: My Code
```python
def valid_str_number(n):
  try: float(n)
  except: return False
  return True
```
