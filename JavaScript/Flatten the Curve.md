## Flatten the Curve

Given an array of integers, replace every number with the average mean of the whole array.
```
Examples
flattenCurve([1, 2, 3, 4, 5]) ➞ [3, 3, 3, 3, 3]

flattenCurve([0, 0, 0, 2, 7, 3]) ➞ [2, 2, 2, 2, 2, 2]

flattenCurve([4]) ➞ [4]

flattenCurve([]) ➞ []

Notes:
Round averages to 1 decimal point.
Return an empty array if given an empty array (see example #4).
```
### :computer: My Code
```js
const flattenCurve = a => a.fill(+(a.reduce((r, n) => r + n, 0) / a.length).toFixed(1));

const flattenCurve = arr => arr.map(a => +((arr.reduce((b,c)=> b + c)) / arr.length).toFixed(1));
  
```
