## X and Y Coordinates

Create a function that converts two lists of x- and y- coordinates into a list of (x,y) coordinates.
```python
Examples
convert_cartesian([1, 5, 3, 3, 4], [5, 8, 9, 1, 0]) 
➞ [[1, 5], [5, 8], [3, 9], [3, 1], [4, 0]]

convert_cartesian([9, 8, 3], [1, 1, 1]) 
➞ [[9, 1], [8, 1], [3, 1]]

Notes:
Each coordinate is a list, not a tuple.
```
### :snake: My Code
```python
convert_cartesian = lambda x, y:[list(a) for a in zip(x,y)]
```
