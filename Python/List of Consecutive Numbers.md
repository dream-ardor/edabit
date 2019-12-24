## List of Consecutive Numbers

Implement a function that returns a list containing all the consecutive numbers in ascendant order from the given value low up to the given value high (bounds included).
```python
Examples
get_sequence(1, 5) ➞ [1, 2, 3, 4, 5]

get_sequence(98, 100) ➞ [98, 99, 100]

get_sequence(1000, 1000) ➞ [1000]
```
### :snake: My Code
```python
get_sequence = lambda l,h: list(range(l, h + 1))
```
