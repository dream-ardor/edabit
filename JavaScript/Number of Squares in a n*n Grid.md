## Number of Squares in a n * n Grid

Create a function that calculates the number of different squares in an n * n square grid. Check the Resources tab.
```js
Examples
numberSquares(2) ➞ 5

numberSquares(4) ➞ 30

numberSquares(5) ➞ 55
```
### :computer: My Code
```js
let numberSquares = n => [...Array(n).keys()].map(x => ++x**2)
 .reduce((a,b)=> a+b);
```
