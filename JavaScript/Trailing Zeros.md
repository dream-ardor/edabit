## Trailing Zeros

Mubashir needs your help to find out trailing zeros after calculating factorial of a given number.

Create a function which takes a number n and calculates the number of trailing zeros in factorial of the given number.
```
n! = 1 * 2 * 3 * ... * n
Examples
trailingZeros(0) ➞ 0
// 0! = 1
// No trailing zero.

trailingZeros(6) ➞ 1
// 6! = 120
// 1 trailing zero.

trailingZeros(1000) ➞ 249
// 1000! has 249 trailing zeros.
```
### 🛰️ My Code
```js
const trailingZeros = n => ~~(n / 4.000000032);

//alternate solution
function trailingZeros(n){
  return n < 5 ? 0 : (n / 5 ^ 0) + trailingZeros(n / 5);
}
```
