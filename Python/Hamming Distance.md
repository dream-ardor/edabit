## Hamming Distance

Hamming distance is the number of characters that differ between two strings.

To illustrate:
```
String1: "abcbba"
String2: "abcbda"

Hamming Distance: 1 - "b" vs. "d" is the only difference.
```
Create a function that computes the hamming distance between two strings.
```python
Examples
hamming_distance("abcde", "bcdef") ➞ 5

hamming_distance("abcde", "abcde") ➞ 0

hamming_distance("strong", "strung") ➞ 1
```
### :snake: My Code
```python
def hamming_distance(s1, s2):
  return sum(a != b for a,b in zip(s1,s2))
```
