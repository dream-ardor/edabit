## Vowel Replacer

Create a function that replaces all the vowels in a string with a specified character.
```python
Examples
replace_vowels("the aardvark", "#") ➞ "th# ##rdv#rk"

replace_vowels("minnie mouse", "?") ➞ "m?nn?? m??s?"

replace_vowels("shakespeare", "*") ➞ "sh*k*sp**r*"
```
### :snake: My Code
```python
def replace_vowels(t,c):
  return ''.join(a if a not in 'aeiou' else c for a in t)
```
