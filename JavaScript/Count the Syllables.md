## Count the Syllables

Create a function that returns the number of syllables in a simple string. The string is made up of short repeated words like "Lalalalalalala" (which would have 7 syllables).
```js
Examples
countSyllables("Hehehehehehe") ➞ 6

countSyllables("bobobobobobobobo") ➞ 8

countSyllables("NANANA") ➞ 3
```
```
Notes
Your code should accept strings of any case (upper, lower and mixed case).
```
### :leaves: My Code
```js
const countSyllables = s => s.match(/.{2}/g).length;
```
