## Double Factorial

Create a function that takes a number num and returns its double factorial.
```
Examples
doubleFactorial(0) ➞ 1

doubleFactorial(2) ➞ 2

doubleFactorial(9) ➞ 945

doubleFactorial(14) ➞ 645120

Notes:
Assume all input values are greater than or equal to -1.
Try to solve it with recursion.
Double factorial is not the same as factorial * 2.
```
### :computer: My Code
```js
const doubleFactorial = n => n < 2 ? 1 : n * doubleFactorial(n-2);
```
