## Sum Of 2 Digit Numbers

For this challenge, you are supposed to find the sum of the digits of a 2 digit number. Sounds easy, right? But for this challenge, I expect you to find the sum of the digits mathematically. Sure you can convert the number into a string and then manipulate it so that it returns the sum of the digits but the point of this challenge is to see if you know how to return the sum of the digits of a two digit number mathematically.
```js
Examples
twoDigitSum(45) ➞ 9

twoDigitSum(38) ➞ 11

twoDigitSum(67) ➞ 13
```
### :deciduous_tree: My Code
```js
const twoDigitSum = n => n % 10 + ~~(n/10);
```
