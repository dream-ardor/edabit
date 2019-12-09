## Binary to Decimal Converter

You are given one input: An array containing eight 1's and/or 0's. Write a function that takes an 8 bit binary number and convert it to decimal.
```js
Examples
binaryToDecimal([1, 1, 1, 1, 1, 1, 1, 1]) ➞ 255

binaryToDecimal([0, 0, 0, 0, 0, 0, 0, 0]) ➞ 0

binaryToDecimal([1, 0, 1, 1, 1, 1, 0, 0]) ➞ 188
```
### :maple_leaf: My Code
```js
let binaryToDecimal = b => parseInt(b.join(''),2);

//alternatively
let binaryToDecimal = b => {
  a = b.toString().split(',').join('');
  return parseInt(a,2);
}
```
