## RegEx Exercise 3: Find all numbers
```js
Challenge:
Write a regexp that looks for all decimal numbers including integer ones, with the floating point and negative ones.
const REGEXP = /your regexp/g

let str = "-1.5 0 2 -123.4."

str.match(REGEXP)  ➞ -1.5, 0, 2, -123.4
```
### :herb: My Code
```js
const REGEXP = /-?\d+(\.\d+)?/g
```
