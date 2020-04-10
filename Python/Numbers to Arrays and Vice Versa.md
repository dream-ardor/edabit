## Numbers to Arrays and Vice Versa
```python
Write two functions:

to_list(), which converts a number to a list of its digits.
to_number(), which converts a list of digits back to its number.

Examples
to_list(235) ➞ [2, 3, 5]

to_list(0) ➞ [0]

to_number([2, 3, 5]) ➞ 235

to_number([0]) ➞ 0
```
### :snake: My Code
```python
to_list = lambda n:[int(x) for x in str(n)]
to_number = lambda l:int("".join([str(i) for i in l] ))

#alternate
to_list = lambda n: list(map(int, str(n)))
to_number = lambda l: int(''.join(map(str, l)))
```
