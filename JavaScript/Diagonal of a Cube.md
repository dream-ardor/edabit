## Diagonal of a Cube

Create a function that takes the volume of a cube and returns the length of the cube's main diagonal, rounded to two decimal places.
```js
Examples
cubeDiagonal(8) ➞ 3.46

cubeDiagonal(343) ➞ 12.12

cubeDiagonal(1157.625) ➞ 18.19
```
### 🔳 My Code
```js
const cubeDiagonal = v => +(3 ** .5 * v ** (1/3)).toFixed(2);
```
