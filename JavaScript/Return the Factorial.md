## Return the Factorial
Create a function that takes an integer and returns the factorial of that integer. That is, the integer multiplied by all positive lower integers.
```js
Examples
factorial(3) ➞ 6

factorial(5) ➞ 120

factorial(13) ➞ 6227020800
```
### :hourglass:My Code
```js
function factorial(int) {
 if (int === 0 || int === 1) {
  return 1;
 }
 for (let i = int -1; i >= 1; i--) {
  int *= i
 }
 return int;
}
```
