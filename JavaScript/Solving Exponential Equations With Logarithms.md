## Solving Exponential Equations With Logarithms

Create a function that takes a number a and finds the missing exponent x so that a when raised to the power of x is equal to b.
```js
Examples
solveForExp(4, 1024) ➞ 5

solveForExp(2, 1024) ➞ 10

solveForExp(9, 3486784401) ➞ 10
```
### :fallen_leaf: My Code
```js
const solveForExp = (a,b) =>
 Math.round(Math.log(b)/ Math.log(a));
```
