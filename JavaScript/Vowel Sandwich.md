## Vowel Sandwich

Create a function which validates whether a 3 character string is a vowel sandwich. In order to have a valid sandwich, the string must satisfy the following rules:

The first and last characters must be a consonant.
The character in the middle must be a vowel.
```js
Examples
isVowelSandwich("cat") ➞ true

isVowelSandwich("ear") ➞ false

isVowelSandwich("bake") ➞ false

isVowelSandwich("try") ➞ false
```
### :sunny: My Code
```js
const isVowelSandwich = s => /^[^aeiou][aeiou][^aeiou]$/.test(s);
```
