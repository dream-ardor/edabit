## Return Last Index

Create a function that returns the last value of the last item in a list or string.
```python
Examples
last_ind([0, 4, 19, 34, 50, -9, 2]) ➞ 2

last_ind("The quick brown fox jumped over the lazy dog") ➞ "g"

last_ind([]) ➞ None
```
### :snake: My Code
```python
last_ind = lambda a:a[-1] if a else None
```
