## Repeating Letters

Create a function that takes a string and returns a string in which each character is repeated once.
```python
Examples
double_char("String") ➞ "SSttrriinngg"

double_char("Hello World!") ➞ "HHeelllloo  WWoorrlldd!!"

double_char("1234!_ ") ➞ "11223344!!__  "
```
## :snake: My Code
```python
def double_char(t):
  return ''.join(i*2 for i in t)
```
