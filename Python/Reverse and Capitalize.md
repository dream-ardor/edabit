## Reverse and Capitalize

Create a function that takes a string of lowercase characters and returns that string reversed and capitalized.
```python
Examples
reverse_capitalize("abc") ➞ "CBA"

reverse_capitalize("hellothere") ➞ "EREHTOLLEH"

reverse_capitalize("input") ➞ "TUPNI"
```
### :snake: My Code
```python
def reverse_capitalize(t):
  return t[::-1].upper()
```
