## Return the First and Last Elements in a List
Create a function that takes a list of elements and return the first and last elements as a new list.
```python
Examples
first_last([5, 10, 15, 20, 25]) ➞ [5, 25]

first_last(["edabit", 13, None, False, True]) ➞ ["edabit", True]

first_last([None, 4, "6", "hello", None]) ➞ [None, None]
```
### :rice:My Code
```python
def first_last(lst):
	return [lst[0],lst[-1]];
```
