## Array of Multiples

Create a function that takes two numbers as arguments (num, length) and returns an array of multiples of num up to length.
```js
Examples
arrayOfMultiples(7, 5) ➞ [7, 14, 21, 28, 35]

arrayOfMultiples(12, 10) ➞ [12, 24, 36, 48, 60, 72, 84, 96, 108, 120]

arrayOfMultiples(17, 6) ➞ [17, 34, 51, 68, 85, 102]

Notes:
Notice that num is also included in the returned array.
```
### :computer: My Code
```js
const arrayOfMultiples = (a,b) => 
 [...Array(b).keys()].map(x => ++x*a);

const arrayOfMultiples = (n,N) =>
 Array.from({ length: N }, (_, i) => n * (i + 1));
 
 //alternate solution
const arrayOfMultiples = (n,N) =>
 [...Array(N).keys()].map((a, b) => n * (b + 1));
```
