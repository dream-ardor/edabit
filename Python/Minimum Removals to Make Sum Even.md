## Minimum Removals to Make Sum Even

Create a function that returns the minimum number of elements removed to make the sum of all elements in a list even.
```
Examples
minimum_removals([1, 2, 3, 4, 5]) ➞ 1

minimum_removals([5, 7, 9, 11]) ➞ 0

minimum_removals([5, 7, 9, 12]) ➞ 1
```
### 🐍 My Code
```python
minimum_removals = lambda l:sum(l) % 2
```
