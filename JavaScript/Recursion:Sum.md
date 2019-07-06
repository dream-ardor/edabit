## Recursion: Sum
Write a function that recursively finds the sum of the first n natural numbers.
```js
Examples
sum(5) ➞ 15
// 1 + 2 + 3 + 4 + 5 = 15

sum(1) ➞ 1

sum(12) ➞ 78
```
### :battery:My Code
```js
const sum = n => n === 1 ? n : n + sum(n-1);
```
