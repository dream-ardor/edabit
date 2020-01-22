## Give Me the Even Numbers

Create a function that takes two parameters (start, stop), and returns the sum of all even numbers in the range.
```python
Examples
sum_even_nums_in_range(10, 20) ➞ 90
# 10, 12, 14, 16, 18, 20

sum_even_nums_in_range(51, 150) ➞ 5050

sum_even_nums_in_range(63, 97) ➞ 1360
```
### :snake: My Code
```python
def sum_even_nums_in_range(a, b):
  return sum(i for i in range(a,b+1) if i % 2 == 0)
```
