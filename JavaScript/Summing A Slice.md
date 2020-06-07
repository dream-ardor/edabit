Summing a Slice

Given an array and an integer n, return the sum of the first n numbers in the array.
```js
Examples
sliceSum([1, 3, 2], 2) ➞ 4

sliceSum([4, 2, 5, 7], 4) ➞ 18

sliceSum([3, 6, 2], 0) ➞ 0
```
### :sunny: My Code
```js
const sliceSum = (a,b) => a.slice(0,b).reduce((a,b)=> a+b, 0);
```
