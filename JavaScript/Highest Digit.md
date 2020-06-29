## Highest Digit

Create a function that takes a number as an argument and returns the highest digit in that number.
```js
Examples
highestDigit(379) ➞ 9

highestDigit(2) ➞ 2

highestDigit(377401) ➞ 7
```
### :sunny: My Code
```js
const highestDigit = n => Math.max(...(''+n));
```
