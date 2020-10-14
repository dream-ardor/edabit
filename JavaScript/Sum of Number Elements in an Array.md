## Sum of Number Elements in an Array

Arrays can be mixed with various types. Your task for this challenge is to sum all the number elements in the given array. Create a function that takes an array and returns the sum of all numbers in the array.
```js
Examples
numbersSum([1, 2, "13", "4", "645"]) ➞ 3

numbersSum([true, false, "123", "75"]) ➞ 0

numbersSum([1, 2, 3, 4, 5, true]) ➞ 15
```
### :computer: My Code
```js
const numbersSum = a => a.filter(x => +x === x).reduce((a,b) => a+b, 0);

//alternate solutions
const numbersSum = r => r.reduce((t, c) => t + (+c === c ? c : 0), 0);

const numbersSum = a => a.filter(x => typeof x == 'number').reduce((a,b) => a+b, 0);
```
