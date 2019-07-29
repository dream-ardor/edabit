## Next Element in Arithmetic Sequence
Create a function that returns the next element in an arithmetic sequence. In an arithmetic sequence, each element is formed by adding the same constant to the previous element.
```python
Examples
next_element([3, 5, 7, 9]) ➞ 11

next_element([-5, -6, -7]) ➞ -8

next_element([2, 2, 2, 2, 2]) ➞ 2
```
### :snake:My Code
```python
def next_element(lst):
	return (lst[-1] - lst[-2]) + lst[-1]
```

## Hashes and Pluses
Create a function that returns the number of hashes and pluses in a string.
```python
Examples
hash_plus_count("###+") ➞ [3, 1]

hash_plus_count("##+++#") ➞ [3, 3]

hash_plus_count("#+++#+#++#") ➞ [4, 6]

hash_plus_count("") ➞ [0, 0]
```
## :snake:My Code
```python
def hash_plus_count(txt):
	h = txt.count("#", 0)
	p = txt.count("+", 0)
	return [h,p]
```

## String or Integer?
Create a function that checks if the argument is an integer or a string.

If it's an integer, return "int"
If it's a string, return "str"
```python
Examples
int_or_string(3) ➞ "int"

int_or_string("Hello") ➞ "str"

int_or_string(8) ➞ "int"

int_or_string("Yo") ➞ "str"

int_or_string(9843532) ➞ "int"
```
### :snake:My Code
```python
def int_or_string(var):
	if type(var) == int: return "int"
	else: return "str"
```

## Truthy or Falsy?
In Python, a truthy value is a value that translates to True when evaluated in a Boolean context. All values are truthy unless they're defined as falsy.

All falsy values are as follows:
```
False
None
0
[]
{}
""
```
Create a function that takes an argument of any data type and returns 1 if it's truthy and 0 if it's falsy.
```python
Examples
is_truthy(0) ➞ 0

is_truthy(False) ➞ 0

is_truthy("") ➞ 0

is_truthy("False") ➞ 1
```
### :snake:My Code
```python
def is_truthy(val):
  if bool(val) == true: return 1
  else: return 0
```

## Find the Index (Part 2)
Create a function that finds the index of a given item if the list is sorted.
```python
Examples
search([1, 2, 3, 4], 3) ➞ 2

search([2, 4, 6, 8, 10], 8) ➞ 3

search([1, 3, 5, 7, 9], 11) ➞ -1
```
Notes
If the item is not present, return -1.
### :snake:My Code
```python
def search(lst, item):
	return lst.index(item) if item in lst else -1
```

## Total Volume
Given a list of boxes, create a function that returns the total volume of all those boxes combined together. A box is represented by a list with three elements: length, width and height.

For instance, total_volume([2, 3, 2], [6, 6, 7], [1, 2, 1]) should return 266 since (2 x 3 x 2) + (6 x 6 x 7) + (1 x 2 x 1) = 12 + 252 + 2 = 266.
```python
Examples
total_volume([4, 2, 4], [3, 3, 3], [1, 1, 2], [2, 1, 1]) ➞ 63

total_volume([2, 2, 2], [2, 1, 1]) ➞ 10

total_volume([1, 1, 1]) ➞ 1
```
### :snake:My Code
```python
def total_volume(*boxes):
	return sum((x*y*z for x,y,z in boxes))
```

## First and Last Index
Given a word, write a function that returns the first index and the last index of a character.
```python
Examples
char_index("hello", "l") ➞ [2, 3]
# The first "l" has index 2, the last "l" has index 3.

char_index("circumlocution", "c") ➞ [0, 8]
# The first "c" has index 0, the last "c" has index 8.

char_index("happy", "h") ➞ [0, 0]
# Only one "h" exists, so the first and last index is 0.

char_index("happy", "e") ➞ None
# "e" does not exist in "happy", so we return undefined.
```
### :snake:My Code
```python
def char_index(word, char):
  if char in word:
	  return [word.index(char), word.rindex(char)]
```
## Is the Number Symmetrical?
Create a function that takes a number as an argument and returns True or False depending on whether the number is symmetrical or not. A number is symmetrical when it is the same as its reverse.
```python
Examples
is_symmetrical(7227) ➞ True

is_symmetrical(12567) ➞ False

is_symmetrical(44444444) ➞ True

is_symmetrical(9939) ➞ False

is_symmetrical(1112111) ➞ True
```
### :snake:My Code
```python
def is_symmetrical(num):
  return str(num) == str(num)[::-1]
```





