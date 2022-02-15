## Is the Dictionary Empty?
Write a function that returns True if a dictionary is empty, and False otherwise.
```python
Examples
is_empty({}) ➞ True

is_empty({ "a": 1 }) ➞ False
```
### :candy: My Code
```python
def is_empty(dict):
  if not dict:
   return True
  else:
   return False
```
