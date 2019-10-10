## Calculate the Median
Create a function that takes an array of numbers and return its median. If the input array is even length, take the average of the two medians, else, take the single median.
```js
Examples
median([2, 5, 6, 2, 6, 3, 4]) ➞ 4

median([21.4323, 432.54, 432.3, 542.4567]) ➞ 432.4

median([-23, -43, -29, -53, -67]) ➞ -43
```
### :computer: My Code
```js
const median = a => {
  a.sort((a,b)=> a-b);
  let b = a.length/2;
  return b % 1 == 0 ? (a[b-1] + a[b]) / 2 : a[Math.floor(b)];
}
```
