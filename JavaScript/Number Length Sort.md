## Number Length Sort

Create a sorting function which sorts numbers not by numerical order, but by number length! This means sorting numbers with the least amount of digits first, up to the numbers with the most digits.
```js
Examples
numberLenSort([1, 54, 1, 2, 463, 2]) ➞ [1, 1, 2, 2, 54, 463]

numberLenSort([999, 421, 22, 990, 32]) ➞ [22, 32, 999, 421, 990]

numberLenSort([9, 8, 7, 6, 5, 4, 31, 2, 1, 3]) ➞ [9, 8, 7, 6, 5, 4, 2, 1, 3, 31]
```
### :palm_tree: My Code
```js
const numberLenSort = arr => arr.sort((a, b) => `${a}`.length - `${b}`.length);

//alternate solutions
const numberLenSort = arr => arr.sort((a, b) => String(a).length - String(b).length);

const numberLenSort = a => a.map(b => String(b)).sort((c,d)=> c.length-d.length).map(Number);
```
