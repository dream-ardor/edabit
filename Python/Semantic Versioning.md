## Semantic Versioning

In semantic versioning a piece of software can be represented in a format like this example: 6.1.9.

The first number is the major version.
The second number is the minor version.
The third number is the patch (bug fixes).
Create three separate functions, one to retrieve each element in the semantic versioning specification.
```python
Examples
# 6.1.9
retrieve_major("6.1.9") ➞ "6"

retrieve_minor("6.1.9") ➞ "1"

retrieve_patch("6.1.9") ➞ "9"

# 2.1.0
retrieve_major("2.1.0") ➞ "2"

retrieve_minor("2.1.0") ➞ "1"

retrieve_patch("2.1.0") ➞ "0"
```
### :snake: My Code
```python
retrieve_major = lambda s:s[0]
retrieve_minor = lambda s:s.split('.')[1]
retrieve_patch = lambda s:s.split('.')[2]
```
