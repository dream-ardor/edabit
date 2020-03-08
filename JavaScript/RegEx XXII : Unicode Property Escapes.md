## RegEx XXII : Unicode property escapes

Unicode property escapes match characters based on their Unicode properties - Binary ("boolean-like") or non-binary. They can be used to match emojis, punctuations, letters (even letters from specific languages or scripts), etc.
```js
const sentence = "A ticket to 大阪 costs ¥2000 👌.";

sentence.match(/\p{Emoji_Presentation}/gu) ➞ ["👌"]
Note: For Unicode property escapes to work, a regular expression must use the u flag which indicates a string must be considered as a series of Unicode code points. See also RegExp.prototype.unicode.

Note: Some Unicode properties encompasses much more characters than some character classes (such as \w which matches only latin letters, a to z) but the latter is better supported among browsers (as of January 2020).
```
#### Challenge
```js
Match all words in the nonEnglishText using a unicode property escape
const nonEnglishText = "Приключения Алисы в Стране чудес";

const regex = /\w+/gu
nonEnglishText.match(regex) ➞ null, \w doesn't work with non english text
 
const regexpBMPWord = /([\u0000-\u0019\u0021-\uFFFF])+/gu;
nonEnglishText.match(regexpBMPWord) ➞ [ 'Приключения', 'Алисы', 'в', 'Стране', 'чудес' ], this works

const regexpUPE = /YOUR SOLUTION HERE/gu;
nonEnglishText.match(regexpUPE) ➞ [ 'Приключения', 'Алисы', 'в', 'Стране', 'чудес' ], an easier way
```
### :computer: My Code
```js
const regexpUPE = /\p{L}+/gu
```
