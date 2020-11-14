## Extend the Vowels

Create a function that takes a word and extends all vowels by a number num.
```js
Examples
extendVowels("Hello", 5) ➞ "Heeeeeelloooooo"

extendVowels("Edabit", 3) ➞ "EEEEdaaaabiiiit"

extendVowels("Extend", 0) ➞ "Extend"

Notes:
Return "invalid" if num isn't 0 or a positive integer.
```
### :leaves: My Code
```js
const extendVowels = (w,n) => n < 0 || n % 1 ? 'invalid' : w.replace(/[aeiou]/ig, a => a.repeat(n+1));
```
