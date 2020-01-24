## Count Ones in Binary Representation of Integer

Count the amount of ones in the binary representation of an integer. So for example, since 12 is '1100' in binary, the return value should be 2.
```python
Examples
count_ones(0) ➞ 0

count_ones(100) ➞ 3

count_ones(999) ➞ 8
```
### :snake: My Code
```python
count_ones = lambda n: bin(n).count('1')
```
