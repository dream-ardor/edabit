## Less Than 100 Array Remix

Given an array of numbers, return true if the sum of the array is less than 100; otherwise return false.
```js
Examples
arrayLessThan100([5, 57]) ➞ true

arrayLessThan100([77, 30]) ➞ false

arrayLessThan100([0]) ➞ true
```
### :sunny: My Code
```js
const arrayLessThan100 = a => a.reduce((b,c) => b+c) < 100;
```
