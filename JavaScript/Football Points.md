## Football Points

Create a function that takes the number of wins, draws and losses and calculates the number of points a football team as obtained so far. A win receives 3 points, a draw 1 point and a loss 0 points.
```js
Examples
footballPoints(3, 4, 2) ➞ 13

footballPoints(5, 0, 2) ➞ 15

footballPoints(0, 0, 1) ➞ 0
```
### :football: My Code
```js
const footballPoints = (a,b,c) => a * 3 + b;
```
