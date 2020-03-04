## Harshad Numbers

A number n is a Harshad (also called Niven) number if it is divisible by the sum of its digits. For example, 666 is divisible by 6 + 6 + 6, so it is a Harshad number.
```js
Examples
isHarshad(209) ➞ true

isHarshad(41) ➞ false

isHarshad(12255) ➞ true
```
### :computer: My Code
```js
const isHarshad = n => n % String(n).match(/\d/g).reduce((a,b)=> +a + +b) == 0;
```
