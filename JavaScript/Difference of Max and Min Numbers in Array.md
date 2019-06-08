## Difference of Max and Min Numbers in Array

Create a function that takes an array and returns the difference between the smallest and biggest numbers.
```js
Examples
differenceMaxMin([10, 4, 1, 4, -10, -50, 32, 21]) ➞ 82
// Smallest number is -50, biggest is 32.

differenceMaxMin([44, 32, 86, 19]) ➞ 67
// Smallest number is 19, biggest is 86.
```
## My Code
```js
const differenceMaxMin = arr => Math.max(...arr) - Math.min(...arr);

```
