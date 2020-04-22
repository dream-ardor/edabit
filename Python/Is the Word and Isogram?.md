## Is the Word an Isogram?

An isogram is a word that has no repeating letters, consecutive or nonconsecutive. Create a function that takes a string and returns either True or False depending on whether or not it's an "isogram".
```python
Examples
is_isogram("Algorism") ➞ True

is_isogram("PasSword") ➞ False
# Not case sensitive.

is_isogram("Consecutive") ➞ False
```
### :snake: My Code
```python
is_isogram = lambda t:len(t) == len(set(t.lower()))
```
