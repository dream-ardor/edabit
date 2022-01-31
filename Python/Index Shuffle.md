## Index Shuffle

Write a function that takes all even-indexed characters and odd-indexed characters from a string and concatenates them together.

To illustrate:
```python
index_shuffle("abcd") ➞ "acbd"
// "ac" (even-indexed) + "bd" (odd-indexed)

Examples
index_shuffle("abcdefg") ➞ "acegbdf"

index_shuffle("holiday") ➞ "hldyoia"

index_shuffle("maybe") ➞ "myeab"
```
### 🐍 My Code
```python
index_shuffle = lambda t:t[::2] + t[1::2]
```
