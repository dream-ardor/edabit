## Sum of Two Numbers in Array Equal to Given Number

Create a function that takes an array of numbers arr and a number n. Return true if the sum of any two elements is equal to the given number. Otherwise, return false.
```js
Examples
checkSum([10, 12, 4, 7, 9, 11], 16) ➞ true

checkSum([4, 5, 6, 7, 8, 9], 13) ➞ true

checkSum([0, 98, 76, 23], 174) ➞ true

checkSum([0, 9, 7, 23, 19, 18, 17, 66], 39) ➞ false

checkSum([2, 8, 9, 12, 45, 78], 1) ➞ false
```
### :leaves: My Code
```js
const checkSum = (a,n) => a.some((b,c) => a.slice(c+1).includes(n-b));

//alternate solution
const checkSum = (arr, n) => arr.some(a => arr.includes(n-a));

const checkSum = (arr, n) => (arr.some((a, i) => arr.some((b, j) => (i !== j) && (a + b === n))));
```
