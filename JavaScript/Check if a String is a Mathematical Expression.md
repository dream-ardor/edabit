## Check if a String is a Mathematical Expression

Create a function that takes an input (e.g. "5 + 4") and returns true if it's a mathematical expression or false if not.
```js
Examples
mathExpr("4 + 5") ➞ true

mathExpr("4*6") ➞ true

mathExpr("4*no") ➞ false
```
### :computer: My Code
```js
const mathExpr = e => /\d+\W+/.test(e);
```
