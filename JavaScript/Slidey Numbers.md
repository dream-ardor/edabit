## Slidey Numbers

A number can considered slidey if for every digit in the number, the next digit from that has an absolute difference of one. Check the examples below.
```js
Examples
isSlidey(123454321) ➞ true

isSlidey(54345) ➞ true

isSlidey(987654321) ➞ true

isSlidey(1123) ➞ false

isSlidey(1357) ➞ false
```
```
Notes
A number cannot slide properly if there is a "flat surface" (example #4), or has gaps! (example #5).
All single digit numbers can be considered slidey numbers!
```
### :computer: My Code
```js
const isSlidey = n => {
  let a = [...n+''].map(Number);
  let b = [];
    for (i = 1; i < a.length; i++) b.push(a[i] - a[i - 1]);
     return b.every(x => x == 1 || x == -1);
}

//alternate
const isSlidey = (n, N = '' + n) =>
  [...N].slice(1).every((v,i) => Math.abs(v - N[i]) === 1);
```
