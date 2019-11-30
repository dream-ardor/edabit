## Find the Missing Number

Create a function that takes a list of numbers between 1 and 10 (excluding one number) and returns the missing number.
```python
Examples
missing_num([1, 2, 3, 4, 6, 7, 8, 9, 10]) ➞ 5

missing_num([7, 2, 3, 6, 5, 9, 1, 4, 8]) ➞ 10

missing_num([10, 5, 1, 2, 4, 6, 8, 3, 9]) ➞ 7
```
### :turkey: My Code
```python
def missing_num(l):
  return [i for i in range(1,11) if i not in l][0]
```
