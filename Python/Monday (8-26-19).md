## Unlucky 13
Given a sorted list of numbers, remove any numbers that are divisible by 13. Return the amended list.
```
Examples
unlucky_13([53, 182, 435, 591, 637]) ➞ [53, 435, 591]
# 182 and 637 are divisible by 13.

unlucky_13([24, 316, 393, 458, 1279]) ➞ [24, 316, 393, 458, 1279]
# No numbers in the list are divisible by 13.

unlucky_13([104, 351, 455, 806, 871]) ➞ []
# All numbers in the list are divisible by 13.
```
### :snake: My Code
```python
def unlucky_13(n):
  return [x for x in n if x % 13]
```
## Filter Repeating Character Strings
Create a function that keeps only strings with repeating identical characters (in other words, it has a set size of 1).
```python
Examples
identical_filter(["aaaaaa", "bc", "d", "eeee", "xyz"])
➞ ["aaaaaa", "d", "eeee"]

identical_filter(["88", "999", "22", "545", "133"])
➞ ["88", "999", "22"]

identical_filter(["xxxxo", "oxo", "xox", "ooxxoo", "oxo"])
➞ []
```
### :snake: My Code
```python
def identical_filter(l):
  return [x for x  in l if len(set(x)) == 1]	
```

