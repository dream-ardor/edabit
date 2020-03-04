## Simon Says

Create a function that takes in two lists and returns True if the second list follows the first list by one element, and False otherwise. In other words, determine if the second list is the first list shifted to the right by 1.
```python
Examples
simon_says([1, 2], [5, 1]) ➞ True

simon_says([1, 2], [5, 5]) ➞ False

simon_says([1, 2, 3, 4, 5], [0, 1, 2, 3, 4]) ➞ True

simon_says([1, 2, 3, 4, 5], [5, 5, 1, 2, 3]) ➞ False
```
### :snake: My Code
```python
simon_says = lambda l1, l2: l1[0] - l2[1]
```
