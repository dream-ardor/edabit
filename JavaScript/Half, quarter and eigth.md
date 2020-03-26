## Half, quarter, and eighth

Create a function that takes a number and return an array of tree numbers: the half of the number, the quarter of the number and the eighth of the number.
```js
Examples
halfQuarterEighth(6) ➞ [ 3, 1.5, 0.75 ]

halfQuarterEighth(22) ➞ [ 11, 5.5, 2.75 ]

halfQuarterEighth(25) ➞ [ 12.5, 6.25, 3.125 ]
```
### :leaves: My Code
```js
const halfQuarterEighth = n => [n/2, n/4, n/8];
```
