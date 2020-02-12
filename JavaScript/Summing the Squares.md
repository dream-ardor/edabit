## Summing the Squares

Create a function where given the number n, return the sum of all square numbers up to and including n.
```js
squaresSum(3) ➞ 14
// 1² + 2² + 3² =
// 1 + 4 + 9 =
// 14 
```
```js
Examples
squaresSum(3) ➞ 14

squaresSum(12) ➞ 650

squaresSum(13) ➞ 819
```
Notes: Remember that n is included in the total.
### :leaves: My Code
```js
const squaresSum = n => {
 let sum = 0;
  for(i =1; i <= n; i++) {sum += (i*i)}
   return sum;
}
```
