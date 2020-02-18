## Sum of the Odd Numbers

Create a function which returns the total of all odd numbers up to and including n. n will be given as an odd number.
```js
Examples
addOddToN(5) ➞ 9
// 1 + 3 + 5 = 9

addOddToN(13) ➞ 49

addOddToN(47) ➞ 576
```
```
Notes
Curiously, the answers are all square numbers!
```
### :computer: My Code
```js
const addOddToN = n =>
 Array(n).fill().map((a,b) => b + 1)
  .filter(a => a % 2).reduce((a,b)=> a + b);
```
