## Vowel Sandwich

Create a function which validates whether a 3 character string is a vowel sandwich. In order to have a valid sandwich, the string must satisfy the following rules:

The first and last characters must be a consonant.
The character in the middle must be a vowel.
```python
Examples
is_vowel_sandwich("cat") ➞ True

is_vowel_sandwich("ear") ➞ False

is_vowel_sandwich("bake") ➞ False

Notes:

Return False if the word is not 3 characters in length.
All words will be given in lowercase.
```
### :snake: My Code
```python
is_vowel_sandwich = lambda s:False if len(s) != 3 else s[1] in 'aeiou' and s[0] not in 'aeiou' and s[-1] not in 'aeiou'

#alternate
is_vowel_sandwich = lambda s:[0,1,0] == [1 if a in 'aeiou' else 0 for a in s]
```
