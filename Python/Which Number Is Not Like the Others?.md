## Which Number Is Not like the Others?

Create a function that takes a list of numbers and return the number that's unique.
```python
Examples
unique([3, 3, 3, 7, 3, 3]) ➞ 7

unique([0, 0, 0.77, 0, 0]) ➞ 0.77

unique([0, 1, 1, 1, 1, 1, 1, 1]) ➞ 0
```
### :computer: My Code
```python
def unique(lst):
	return min(set(lst), key=lst.count)
  
 #alternate
 def unique(lst):
	return [num for num in lst if lst.count(num) <= 1][0]

#alternate, O(n) complexity (2 traversals of the list)
def unique(l):
    a = {}

    for b in l:
        if b in a:
            a[b] += 1
        else:
            a[b] = 1

    for b in l:
        if a[b] == 1:
            return b

    return -1
```
