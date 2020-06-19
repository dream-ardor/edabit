## Sum of Decimals

Captain Obvious is asked to implement a simple function that given two decimal numbers A and B returns their sum.

"Easy one!" he thinks, but soon he discovers that his function fails over the fifty percent of given test cases! He suspects the test cases are wrong, but his calculator is saying they're correct! What's happening?

Can you help Captain Obvious to debug his function and solve the exercise?
```js
Examples
floatSum(0.3, 0.7) ➞ 1

floatSum(0.35, 0.75) ➞ 1.1

floatSum(1.234, 5.6789) ➞ 6.9129
```
### :computer: My Code
```js
const floatSum = (a,b) => +(a + b).toFixed(12);
```
