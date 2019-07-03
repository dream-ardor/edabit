## Truthy or Falsy?
In Python, a truthy value is a value that translates to True when evaluated in a Boolean context. All values are truthy unless they're defined as falsy.

All falsy values are as follows:
```
False
None
0
[]
{}
""
```
Create a function that takes an argument of any data type and returns 1 if it's truthy and 0 if it's falsy.
```python
Examples
is_truthy(0) ➞ 0

is_truthy(False) ➞ 0

is_truthy("") ➞ 0

is_truthy("False") ➞ 1
```
### :chocolate_bar:My Code
```python
def is_truthy(val):
	return 1 if bool(val) else 0;
```
