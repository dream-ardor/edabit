## RegEx: Boundary Assertions I

Assume a program only reads .js or .jsx files. Write a function that accepts a file path and returns true if it can read the file and false if it can't.
```js
Examples
isJS("/users/user.jsx") ➞ true

isJS("/users/user.js") ➞ true

isJS("/users/user.ts") ➞ false
```
### :leaves: My Code
```js
const isJS = p => /\b(.)js/.test(p);
```
