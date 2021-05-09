## Simple Letters

Create a function that takes two lowercase strings str1 and str2 of letters from a to z and returns the sorted and longest string containing distinct letters.
```python
Examples
str1 = "mubashir"
str2 = "edabit"

longest_string(str1, str2) ➞ "abdehimrstu"
# Contains sorted and distinct letters of the given strings.

str1 = "abcdefghijklmnopqrstuvwxyz"
str2 = "abcdefghijklmnopqrstuvwxyz"

longest_string(str1, str2) ➞ "abcdefghijklmnopqrstuvwxyz"
# Contains sorted and distinct letters of the given strings.
```
### :snake: My Code
```python
longest_string = lambda a,b:''.join((sorted(set(a+b))))
```
