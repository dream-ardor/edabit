## Find the nth Tetrahedral Number

A tetrahedron is a pyramid with a triangular base and three sides. A tetrahedral number is a number of items within a tetrahedron.

Create a function that takes an integer n and returns the nth tetrahedral number.

```js
Examples
tetra(2) ➞ 4

tetra(5) ➞ 35

tetra(6) ➞ 56
```
### :leaves: My Code
```js
let tetra = n => n * ++n * ++n / 6;

//alternate solution
let tetra = n => (n * (n + 1) * (n + 2)) / 6;
```
