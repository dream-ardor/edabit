## WordCharWord

Create a function that will put the first argument, a character, between every word in the second argument, a string.
```python
Examples
add("#", "hello world!") ➞ "hello#world!"
```
### :snake: My Code
```python
add = lambda c,t:t.replace(' ',c)
```
