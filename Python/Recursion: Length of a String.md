## Recursion: Length of a String

Write a function that returns the length of a string. Make your function recursive.
```python
Examples
length("apple") ➞ 5

length("make") ➞ 4

length("a") ➞ 1

length("") ➞ 0
```
### :snake: My Code
```python
length = lambda t: 0 if t == '' else 1 + length(t[:-1])
```
