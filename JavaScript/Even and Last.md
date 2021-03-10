## Even and Last
Given a array of integers arr, return the sum of all the integers that have an even index, multiplied by the integer at the last index.

If the sequence is empty, you should return 0.
```js
Examples
evenLast([2, 3, 4, 5]) ➞ 30
// numbers at even index = 2, 4
// number at last index = 5
// 2*5 + 4*5 = 10 + 20 = 30

evenLast([1, 3, 3, 1, 10]) ➞ 140

evenLast([]) ➞ 0
```
### :evergreen_tree: My Code
```js
const evenLast = n => n.reduce((a,b,c) => c % 2 ? a : a + b, 0) * n[n.length-1] || 0;

```
