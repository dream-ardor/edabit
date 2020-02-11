## Moving to the End

Write a function that moves all elements of one type to the end of the list.
```python
Examples
move_to_end([1, 3, 2, 4, 4, 1], 1) ➞ [3, 2, 4, 4, 1, 1]
# Move all the 1s to the end of the array.

move_to_end([7, 8, 9, 1, 2, 3, 4], 9) ➞ [7, 8, 1, 2, 3, 4, 9]

move_to_end(["a", "a", "a", "b"], "a") ➞ ["b", "a", "a", "a"]
```
### :snake: My Code
```python
move_to_end = lambda lst, el: sorted(lst,key=lambda x: (x == el))
```
