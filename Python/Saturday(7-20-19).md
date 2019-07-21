## Reverse Coding Challenge #3
This is a reverse coding challenge. Normally you're given explicit directions with how to create a function. Here, you must generate your own function to satisfy the relationship between the inputs and outputs.

Your task is to create a function that, when fed the inputs below, produce the sample outputs shown.
```python
Examples
[5, 7, 8, 2, 1], 2 ➞ [1, 1, 0, 0, 1]

[9, 8, 16, 47], 4 ➞ [1, 0, 0, 3]

[17, 11, 99, 55, 23, 1], 5 ➞ [2, 1, 4, 0, 3, 1]

[6, 1], 7 ➞ [6, 1]

[3, 2, 9], 3 ➞ [0, 2, 0]

[48, 22, 0, 19, 33, 100], 10 ➞ [8, 2, 0, 9, 3, 0]
```
### :beginner:My Code
```python
def mystery_func(lst, n):
  return [item % n for item in lst]
```
## Check if Number is within a Given Range
Given a number and a dictionary with min and max properties, return True if the number lies within the given range (inclusive).
```python
Examples
is_in_range(4, { "min": 0, "max": 5 }) ➞ True

is_in_range(4, { "min": 4, "max": 5 }) ➞ True

is_in_range(4, { "min": 6, "max": 10 }) ➞ False

is_in_range(5, { "min": 5, "max": 5 }) ➞ True
```
### :atm:My Code
```python
def is_in_range(n, r):
  return n >= r['min'] and n <= r['max']
```

## Find the Bug: Checking Even Numbers
Create a function that takes in an array and returns True if all its values are even, and False otherwise.

Not a big deal, your friend says. He writes the following code:
```python
def check_all_even(lst):
  return all(x % 2 == 0)
```
The code above leads to a Reference Error, with x being undefined. Fix the code above so that all tests pass:
```python
Examples
check_all_even([1, 2, 3, 4]) ➞ False

check_all_even([2, 4, 6]) ➞ True

check_all_even([5, 6, 8, 10]) ➞ False

check_all_even([-2, 2, -2, 2]) ➞ True
```
### :apple:My Code
```python
def check_all_even(lst):
  return all(x % 2 == 0 for x in lst)
```

## Palindrome?
A palindrome is a word that is identical forward and backwards.
```
mom
racecar
kayak
```
Given a word, create a function that checks whether it is a palindrome.
```python
Examples
is_palindrome("mom") ➞ True

is_palindrome("scary") ➞ False

is_palindrome("reviver") ➞ True

is_palindrome("stressed") ➞ False
```
### :sweet_potato:My Code
```python
def is_palindrome(txt):
	rev = ''.join(reversed(txt))
	if (rev == txt):
	  return True
	else:
	  return False
	  
#alternate solution
def is_palindrome(txt):
		return txt == txt[::-1]
```








