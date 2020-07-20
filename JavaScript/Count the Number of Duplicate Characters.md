## Count the Number of Duplicate Characters

Create a function that returns the amount of duplicate characters in a string. It will be case sensitive and spaces are included. If there are no duplicates, return 0.
```js
Examples
duplicates("Hello World!") ➞ 3

duplicates("foobar") ➞ 1

duplicates("helicopter") ➞ 1

duplicates("birthday") ➞ 0
// If there are no duplicates, return 0
```
### :sunny: My Code
```js
const duplicates = s => s.length - new Set(s).size;
```
