## Letters Shared between Two Words

Create a function that returns the number of characters shared between two words.
```js
Examples
sharedLetters("apple", "meaty") ➞ 2
// Since "ea" is shared between "apple" and "meaty".

sharedLetters("fan", "forsook") ➞ 1

sharedLetters("spout", "shout") ➞ 4
```
### :sunny: My Code
```js
const sharedLetters = (a,b) => [...new Set(a)].filter(c => b.includes(c)).length;
```
