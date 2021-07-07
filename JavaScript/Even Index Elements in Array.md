## Even Index Elements in Array

Create a function that takes an array of integers and returns the sum of all the integers that have an even index, multiplied by the integer at the last index.

For example:
```js
[2, 3, 4, 5] ➞ 30
(2 + 4) * 5 ➞ 30

[1, 4, 5, 6, 7, 2, 3] ➞ 48
(1 + 5 + 7 + 3) * 3 ➞ 48

Examples
evenLast([]) ➞ 0

evenLast([1, 3, 3, 1, 10]) ➞ 140

evenLast([-11, 3, 3, 1, 10]) ➞ 20
```
### 🌴 My Code
```js
const evenLast = a => a.filter((b,c) => c % 2 == 0).reduce((a,b)=>a+b,0) * a.slice(-1);


//alternate solutions
const evenLast = r => r.reduce((a,c,i) => !(i % 2) ? a + c * r[r.length-1]: a, 0);

const evenLast = arr => arr.reduce((a, b, i) => a + (i%2 ? 0 : b), 0) * arr.pop() || 0;
```
