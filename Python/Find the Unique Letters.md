## Find the Unique Letters

Create a function that takes a string and returns the letters that occur only once.
```python
Examples
find_letters("monopoly") ➞ ["m", "n", "p", "l", "y"]

find_letters("balloon") ➞ ["b", "a", "n"]

find_letters("analysis") ➞ ["n", "l", "y", "i"]
```
### :snake: My Code
```python
find_letters = lambda w:[x for x in w if w.count(x) < 2]
```
