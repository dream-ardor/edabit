## Volume of a Cone
Create a function that takes the height and radius of a cone as arguments and returns the volume of the cone. See the resources tab for the formula.
```python
Examples
cone_volume(3, 2) ➞ 12.57

cone_volume(15, 6) ➞ 565.49

cone_volume(18, 0) ➞ 0
```
### :snake: My Code
```python
import math
cone_volume = lambda h,r : round(math.pi * r**2 * h/3, 2)
```
