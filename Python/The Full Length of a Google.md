## The Full Length of a Google

Google's logo can be stretched depending on how many pages it lets you skip forward to.

Let's say we wanted to change the amount of pages that Google could skip to. Create a function where given a number of pages n, return the word 'Google' but with the correct number of 'o's.
```python
Examples
googlify(10) ➞ 'Goooooooooogle'

googlify(23) ➞ 'Gooooooooooooooooooooooooogle'

googlify(2) ➞ 'Google'

googlify(-2) ➞ 'invalid'

Notes:
If n is equal to or less than 1, return invalid.`
```
### :snake: My Code
```python
googlify = lambda n:'G' + ('o'* n) + 'gle' if n > 1  else 'invalid'
```
