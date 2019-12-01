## Even Number Generator

Using list comprehensions, create a function that finds all even numbers from 1 to the given number.
```python
Examples
find_even_nums(8) ➞ [2, 4, 6, 8]

find_even_nums(4) ➞ [2, 4]

find_even_nums(2) ➞ [2]
```
### :snake: My Code
```python
def find_even_nums(n):
  return [x for x in range(1, n+1) if x % 2 == 0]
  
#alternatively
def find_even_nums(n):
  return [i for i in range(2, n+1, 2)] 
```
