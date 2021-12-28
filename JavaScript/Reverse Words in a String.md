## Reverse Words in a String

Given an input string, reverse the string word by word, the first word will be the last, and so on.
```js
Examples
reverseWords(" the sky is blue") ➞ "blue is sky the"

reverseWords("hello   world!  ") ➞ "world! hello"

reverseWords("a good example") ➞ "example good a"
```
### 🌴 My Code
```js
let reverseWords = s => s.split` `.reverse().join` `;
```
