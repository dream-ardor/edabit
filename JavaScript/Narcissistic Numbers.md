## Narcissistic Numbers
A number is narcissistic when the sum of its digits, with each digit raised to the power of digits quantity, is equal to the number itself.
```
153 ➞ 3 digits ➞ 1³ + 5³ + 3³ = 1 + 125 + 27 = 153 ➞ Narcissistic
84 ➞ 2 digits ➞ 8² + 4² = 64 + 16 = 80 ➞ Not narcissistic
```
Given a positive integer n, implement a function that returns true if the number is narcissistic, and false if it's not.
```js
Examples
isNarcissistic(8208) ➞ true
// 8⁴ + 2⁴ + 0⁴ + 8⁴ = 8208

isNarcissistic(22) ➞ false
// 2² + 2² = 8

isNarcissistic(9) ➞ true
// 9¹ = 9
```
### :jack_o_lantern: My Code
```js
const isNarcissistic = n =>
 [...n+''].map(x => x**[...n+''].length).reduce((a,b)=>a+b) == n;

//alternate
function isNarcissistic(n) {
  let pow = n.toString().split('').map(x => 
    Math.pow(x, n.toString().length));
  let val = pow.reduce((a,b) => a+b);
  return val === n;
};
```
