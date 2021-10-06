## Count Palindrome Numbers in a Range

Create a function that returns the number of palindrome numbers in a specified range (inclusive).

For example, between 8 and 34, there are 5 palindromes: 8, 9, 11, 22 and 33. Between 1550 and 1552 there is exactly one palindrome: 1551.
```python
Examples
count_palindromes(1, 10) ➞ 9

count_palindromes(555, 556) ➞ 1

count_palindromes(878, 898) ➞ 3
```
### :snake: My Code
```python
def count_palindromes(a, b):
 return sum(str(i)==str(i)[::-1] for i in range(a, b + 1))
```
