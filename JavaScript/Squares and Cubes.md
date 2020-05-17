## Squares and Cubes

Create a function that takes an array of two numbers and checks if the square root of the first number is equal to the cube root of the second number.
```js
Examples
checkSquareAndCube([4, 8]) ➞ true

checkSquareAndCube([16, 48]) ➞ false

checkSquareAndCube([9, 27]) ➞ true
```
### :computer: My Code
```js
const checkSquareAndCube = a => Math.sqrt(a[0]) == Math.cbrt(a[1]);
```
