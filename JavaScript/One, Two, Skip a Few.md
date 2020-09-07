## One, Two, Skip a Few

Create a function which calculates how many numbers are missing from an ordered number line.
```js
howManyMissing([1, 2, 3, 8, 9]) ➞ 4

// The number line starts at 1 and ends at 9 (so the numbers 0 and 10 aren't missing from it).
// The numbers missing from this line are 4, 5, 6, and 7.
// 4 numbers are missing.

Examples
howManyMissing([1, 3]) ➞ 1

howManyMissing([7, 10, 11, 12]) ➞ 2

howManyMissing([1, 3, 5, 7, 9, 11]) ➞ 5

howManyMissing([5, 6, 7, 8]) ➞ 0

Notes
If the number line is complete, or the array is empty, return 0.
```
### :leaves: My Code
```js
const howManyMissing = arr => arr.slice(-1) - arr[0] + 1 - arr.length || 0;


//alternate solution 1
const howManyMissing = (arr, L = arr.length) => L ? arr[L-1] - arr[0] + 1 - L : 0;

//alternate solution 2
const howManyMissing = (arr) => arr.slice(1,).reduce((a,x,i) => a + (x - arr[i]-1),0);

//alternate solution 3
const howManyMissing = a => a.length ? Math.max(...a)-Math.min(...a)-a.length+1 : 0;
```
