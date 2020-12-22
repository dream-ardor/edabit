## Outlier Number

Given an array of either entirely odd integers or entirely even integers except for a single Outlier Number. Create a function to return this number.
```js
Examples

outlierNumber([2, 3, 4]) ➞ 3
// 2 & 4 are even numbers.
// 3 is outlier number.

outlierNumber([1, 2, 3]) ➞ 2

outlierNumber([4, 1, 3, 5, 9]) ➞ 4
```
### :evergreen_tree: My Code
```js
const outlierNumber = a => {
  let b = a.filter(a => a % 2 == 0);
  let c = a.filter(a  => a % 2 !== 0);
  return b.length == 1 ? b[0] : c[0];
}
```
