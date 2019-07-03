## Case Insensitive Comparison
Write a function that validates whether two strings are identical. Make this validator case insensitive.
```python
Examples
match("hello", "hELLo") ➞ True

match("motive", "emotive") ➞ False

match("venom", "VENOM") ➞ True

match("mask", "mAskinG") ➞ False
```
### My Code
```python
def match(s1, s2):
	return s1.lower() == s2.lower();
```
