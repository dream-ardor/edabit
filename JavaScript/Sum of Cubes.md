## Sum of Cubes

Create a function that takes a positive integer n, and returns the sum of all the cubed values from 1 to n.

For example, if n is 3:
```js
sumCubes(3) ➞ 36
1 ** 3 + 2 ** 3 + 3 ** 3 = 36
Examples
sumCubes(7)  ➞ 784

sumCubes(8)  ➞ 1296

sumCubes(9)  ➞ 2025
```
### :leaves: My Code
```js
const sumCubes = n => [...Array(n).keys()].map(i => i + 1).reduce((a,b) => b ** 3 + a);
```
