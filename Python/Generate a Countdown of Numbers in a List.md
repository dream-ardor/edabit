## Generate a Countdown of Numbers in a List

Create a function that takes a number as an argument and returns a list of numbers counting down from this number to zero.
```python
Examples
countdown(5) ➞ [5, 4, 3, 2, 1, 0]

countdown(1) ➞ [1, 0]

countdown(0) ➞ [0]
```
### :computer: My Code
```python
countdown = lambda n:list(range(n,-1,-1))

```
