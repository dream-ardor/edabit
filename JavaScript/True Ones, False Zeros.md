## True Ones, False Zeros

Create a function that returns an array of booleans from a given number by iterating through the number one digit at a time and appending true into the array if the digit is 1 and false otherwise.
```js
Examples
integerBoolean("100101") ➞ [true, false, false, true, false, true]

integerBoolean("10") ➞ [true, false]

integerBoolean("001") ➞ [false, false, true]
```
### :computer: My Code
```js
const integerBoolean = n => [...n].map(a => a == 1);
```
