## Square Every Digit

Create a function that squares every digit of a number.
```js
Examples
squareDigits(9119) ➞ 811181

squareDigits(2483) ➞ 416649

squareDigits(3212) ➞ 9414
```
### :leaves: My Code
```js
const squareDigits = n =>
 +n.toString().split('').map(x=>x*x).join('');
 
 //alternative solution
const squareDigits = n => 
 +[...`${n}`].map(x => x*x).join('');
 
```
