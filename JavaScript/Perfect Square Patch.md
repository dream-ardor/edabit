## Perfect Square Patch

Create a function that takes an integer and outputs an n x n square solely consisting of the integer n.
```
Examples: 

squarePatch(3) ➞ [
  [3, 3, 3],
  [3, 3, 3],
  [3, 3, 3]
]

squarePatch(5) ➞ [
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5],
  [5, 5, 5, 5, 5]
]

squarePatch(1) ➞ [
  [1]
]

squarePatch(0) ➞ []
```
### :computer: My Code
```js
const squarePatch = n => Array(n).fill(Array(n).fill(n));
```
