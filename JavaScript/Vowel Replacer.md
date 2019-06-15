## Vowel Replacer

Create a function replaces all the vowels in a string with a specified character.
```js
Examples:
replaceVowels("the aardvark", "#") ➞ "th# ##rdv#rk"

replaceVowels("minnie mouse", "?") ➞ "m?nn?? m??s?"

replaceVowels("shakespeare", "*") ➞ "sh*k*sp**r*"
```

## My Code
```js
const replaceVowels = (str, ch) => str.replace(/[aeiou]/gi, ch)
```
