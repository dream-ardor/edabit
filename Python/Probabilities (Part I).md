## Probabilities (Part 1)

Given a list of numbers and a value n, write a function that returns the probability of choosing a number greater than or equal to n from the list. The probability should be expressed as a percentage, rounded to one decimal place.
```python
Examples
probability([5, 1, 8, 9], 6) ➞ 50.0

probability([7, 4, 17, 14, 12, 3], 16) ➞ 16.7

probability([4, 6, 2, 9, 15, 18, 8, 2, 10, 8], 6) ➞ 70.0
```
### :snake: My Code
```python
def probability(l, n):
  return round((len([i for i in l if i >= n]) / len(l) * 100),1)
```
