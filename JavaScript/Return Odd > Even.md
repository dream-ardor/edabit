## Return Odd > Even

Given an array, return true if there are more odd numbers than even numbers, otherwise return false.
```js
Examples
oddeven([1, 2, 3, 4, 5, 6, 7, 8, 9]) ➞ true

oddeven([1]) ➞ true

oddeven([13452394823795273847528572346]) ➞ false
```
### :computer: My Code
```js
const oddeven = a => a.filter(b => b % 2).length > a.filter(b => b % 2 == 0).length;
```
