## Is It the Same Upside Down?

The number 6090609 has a special property: if you turn the number upside down (imagine rotating your screen 180 degrees), you get 6090609 again.

Write a function that takes a string on the digits 0, 6, 9 and returns true if the number is the same upside down or false otherwise.
```js
Examples
sameUpsidedown("6090609") ➞ true

sameUpsidedown("9669") ➞false
// Becomes 6996 when upside down.

sameUpsidedown("69069069") ➞ true
```
### My Code
```js
//first solution
const sameUpsidedown = s => s == [...s].map(e =>
 ({6: '9', 9: '6', 0: '0'})[e]).reverse().join('');
 
//second solution
const swap69nice = m => m === '6' ? '9' : '6';
const sameUpsidedown = s => (
 s.replace(/[69]/g, swap69nice) === [...s].reverse().join('')
);
  
//third solution
const sameUpsidedown = strNum => {
 return strNum.split('').join('')==strNum.split('').reverse().map(c=>c==6?9:c==9?6:0).join('');
}
```
