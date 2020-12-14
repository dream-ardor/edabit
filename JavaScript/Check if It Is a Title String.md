## Check if It Is a Title String

Check if a string is a title string or not.

A title string is one which has all the words in the string start with a upper case letter.
```js
Examples

"A Mind Boggling Achievement" ➞ true

"A Simple Java Script Program!" ➞ true

"Water is transparent" ➞ false
```
### :cherry_blossom: My Code
```js
let checkTitle = t => t.match(/\b\w/g).map(a => a == a.toUpperCase()).pop();
```
