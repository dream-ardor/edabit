## C String to C++ String (in Python)

This is a list of single characters with an unwanted character at the end:

["H", "e", "l", "l", "o", "!", "\0"]
You could also just type "Hello!" when initializing a variable, creating the string "Hello!"

Create a function that will return a string by combining the given character list, not including the unwanted final character.
```python
Examples
cpp_txt(["H", "i", "!", "\0"]) ➞ "Hi!"

cpp_txt(["H", "e", "l", "l", "o", "!", "\0"]) ➞ "Hello!"

cpp_txt(["J", "A", "V", "a", "\0"]) ➞ "JAVa"
```
### :snake: My Code
```python
cpp_txt = lambda l:''.join(l[:-1])
```
