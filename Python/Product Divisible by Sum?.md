## Product Divisible by Sum?

Write a function that returns True if the product of a list is divisible by the sum of that same list. Otherwise, return False.
```python
Examples
divisible([3, 2, 4, 2]) ➞ False

divisible([4, 2, 6]) ➞ True
# 4 * 2 * 6 / (4 + 2 + 6)

divisible([3, 5, 1]) ➞ False
```
### 🐍 My Code
```python
import numpy
divisible = lambda l:numpy.prod(l) % sum(l) == 0


#alternate solution 
import numpy as m
divisible = lambda l:m.prod(l) % sum(l) == 0
```
