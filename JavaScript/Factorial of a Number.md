## Factorial of a Number

Create a function that receives a non-negative integer and returns the factorial of that number.
```js
Examples
fact(0) ➞ 1

fact(1) ➞ 1

fact(3) ➞ 6

fact(6) ➞ 720
```
### :computer: My Code
```js
const fact = n => n < 2 ? 1 : n * fact(n-1);
```
