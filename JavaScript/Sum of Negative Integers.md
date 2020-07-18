## Sum of Negative Integers

Create a function that takes a string containing integers as well as other characters and return the sum of the negative integers only.
```js
Examples
negativeSum("-12 13%14&-11") ➞ -23
// -12 + -11 = -23

negativeSum("22 13%14&-11-22 13 12") ➞ -33
// -11 + -22 = -33
```
### :computer: My Code
```js
const negativeSum = c => c.match(/\-\d+/g).reduce((a,b)=> a + +b, 0)
```
