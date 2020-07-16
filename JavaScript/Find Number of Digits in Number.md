## Find Number of Digits in Number

Create a function that will return an integer number containing the amount of digits in the given integer num.
```js
Examples
num_of_digits(1000) ➞ 4

num_of_digits(12) ➞ 2

num_of_digits(1305981031) ➞ 10

num_of_digits(0) ➞ 1

Notes
Try to solve this challenge without using strings!
```
### :computer: My Code
```js
const num_of_digits = n => (Math.log10((n ^ (n >> 31)) - (n >> 31)) | 0) + 1;
```
