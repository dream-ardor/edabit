## Reverse and Capitalize

Create a function that takes a string of lowercase characters and returns that string reversed and capitalized.
```js
Examples
reverseCapitalize("abc") ➞ "CBA"

reverseCapitalize("hellothere") ➞ "EREHTOLLEH"

reverseCapitalize("input") ➞ "TUPNI"
```
### :fallen_leaf: My Code
```js
let reverseCapitalize = s => [...s].reverse().join('').toUpperCase();
```
