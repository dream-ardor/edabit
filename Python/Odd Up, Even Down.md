## Odd Up, Even Down

Create a function that goes through the array, incrementing (+1) for each odd number and decrementing (-1) for each even number.
```python
Examples
transform([1, 2, 3, 4, 5]) ➞ [2, 1, 4, 3, 6]

transform([3, 3, 4, 3]) ➞ [4, 4, 3, 4]

transform([2, 2, 0, 8, 10]) ➞ [1, 1, -1, 7, 9]
```
### :snake: My Code
```python
transform = lambda a:[x+1 if x % 2 else x-1 for x in a]
```
