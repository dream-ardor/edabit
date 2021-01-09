## Largest Numbers

Create a function that takes two arguments of a list of numbers lst and a constant number n and returns the n largest numbers from the given list.
```python
Examples

largest_numbers(2, [4, 3, 2, 1]) ➞ [3, 4]

largest_numbers(1, [7, 19, 4, 2]) ➞ [19]

largest_numbers(3, [14, 12, 57, 11, 18, 16]) ➞ [16, 18, 57]

largest_numbers(0, [1, 3, 4, 2]) ➞ []

Notes:

The returned list must be sorted in ascending order.
```
### :snake: My Code
```python
largest_numbers = lambda n,l:sorted(l)[-n:] if n else []
```
