## Divisible by Left Digit?

Create a function which takes a number n and checks if each digit is divisible by the digit on its left. Return a boolean array depending on the condition checks.
```js
Examples
divisibleByLeft(73312) ➞ [false, false, true, false, true]
// no element left to 7 = false
// 3/7 = false
// 3/3 = true
// 1/3 = false
// 2/1 = true

divisibleByLeft(1) ➞ [false]

divisibleByLeft(635) ➞ [false, false, false]

Notes:
Array should always start with false as there is no digit to the left of first digit.
```
### :fallen_leaf: My Code
```js
const divisibleByLeft = n => [...n+= ''].map((a,b)=> a % n[b-1] < 1);
```
