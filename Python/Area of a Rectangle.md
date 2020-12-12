## Area of a Rectangle

Create a function that calculates the area of a rectangle. If the arguments are invalid, your function must return -1.
```python
Examples

area(3, 4) ➞ 12

area(10, 11) ➞ 110

area(-1, 5) ➞ -1

area(0, 2) ➞ -1
```
### :snake: My Code
```python
area = lambda h,w:h * w if h > 0 and w > 0 else -1
```
