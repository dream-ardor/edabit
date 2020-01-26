## Is the String in Order?

Create a function that takes a string and returns True or False, depending on whether the characters are in order or not.
```python
Examples
is_in_order("abc") ➞ True

is_in_order("edabit") ➞ False

is_in_order("123") ➞ True

is_in_order("xyzz") ➞ True
```
### :snake: My Code
```python
is_in_order = lambda t: sorted(t) == list(t)
	
```
