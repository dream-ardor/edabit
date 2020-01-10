## Check for Anagrams
Create a function that takes two strings and returns either True or False depending on whether they're anagrams or not.
```python
Examples
is_anagram("cristian", "Cristina") ➞ True

is_anagram("Dave Barry", "Ray Adverb") ➞ True

is_anagram("Nope", "Note") ➞ False
```
### :snake: My Code
```python
is_anagram = lambda s1, s2:sorted(s1.lower()) == sorted(s2.lower())
```
