## Pyramid Lists

Given a number n, return a list containing several lists. Each list increment in size, from range 1 to n inclusive, contaning its length as the elements.
```python
Examples
pyramid_lists(1) ➞ [[1]]

pyramid_lists(3) ➞ [[1], [2, 2], [3, 3, 3]]

pyramid_lists(5) ➞ [[1], [2, 2], [3, 3, 3], [4, 4, 4, 4], [5, 5, 5, 5, 5]]
```
### :snake: My Code
```python
pyramid_lists = lambda n:[[a] * a for a in range(1, n+1)]
```
