## Regex Series: String Contains at Least One Digit

Write a regular expression that matches a string if it contains at least one digit.
```python
Examples
has_digit("c8") ➞ True

has_digit("23cc4") ➞ True

has_digit("abwekz") ➞ False

has_digit("sdfkxi") ➞ False
```
### :snake: My Code
```python
import re
has_digit = lambda t: bool(re.search('\d', t))
```
