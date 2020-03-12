## Same Parity?

Create a function that takes a number as input and returns true if the sum of its digits has the same parity as the entire number. Otherwise, return false.
```js
Examples
parityAnalysis(243) ➞ true
// 243 is odd and so is 9 (2 + 4 + 3)

parityAnalysis(12) ➞ false
// 12 is even but 3 is odd (1 + 2)

parityAnalysis(3) ➞ true
// 3 is odd and 3 is odd and 3 is odd (3)
```
### :leaves: My Code
```js
const parityAnalysis = n =>
 [...n+''].map(Number).reduce((a,b)=> a+b) % 2 && n % 2 ? true :
 [...n+''].map(Number).reduce((a,b)=> a+b) % 2 == 0 && n % 2 == 0 ? true : false;
```
