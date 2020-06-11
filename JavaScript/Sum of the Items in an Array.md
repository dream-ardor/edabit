## Sum of the Items in an Array

Create a function that takes an array and returns the sum of all items in the array.
```js
Examples
sumArray([1, 2, 3]) ➞ 6
// 1 + 2 + 3 = 6

sumArray([1, [2, [1]], 3]) ➞ 7
// 1 + 2 + 1 + 3 = 7
```
### :computer: My Code
```js
const sumArray = a => a.flat(Infinity).reduce((a,b)=> a+b);
```
