## Return Odd > Even

Given a list, return True if there are more odd numbers than even numbers, otherwise return False.
```python
Examples
oddeven([1, 2, 3, 4, 5, 6, 7, 8, 9]) ➞ True

oddeven([1]) ➞ True

oddeven([13452394823795273847528572346]) ➞ False
```
### :computer: My Code
```python
def oddeven(l):
  return len([a for a in l if a%2]) > len([a for a in l if a%2==0])
  
 #alternate
def oddeven(lst):
  return sum(1 if i % 2 else -1 for i in lst) > 0
```
