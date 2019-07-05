## Absolute Sum
Take an array of integers (positive or negative or both) and return the sum of the absolute value of each element.
```js
Examples
getAbsSum([2, -1, 4, 8, 10]) ➞ 25

getAbsSum([-3, -4, -10, -2, -3]) ➞ 22

getAbsSum([2, 4, 6, 8, 10]) ➞ 30

getAbsSum([-1]) ➞ 1
```
### :fireworks:My Code
```js
const getAbsSum = arr => arr.reduce((a,b)=> Math.abs(a) + Math.abs(b),0);
```

## Total Volume
Given an array of boxes, create a function that returns the total volume of all those boxes combined together. A box is represented by an array with three elements: length, width and height.

For instance, totalVolume([2, 3, 2], [6, 6, 7], [1, 2, 1]) should return 266 since (2 x 3 x 2) + (6 x 6 x 7) + (1 x 2 x 1) = 12 + 252 + 2 = 266.
```js
Examples
totalVolume([4, 2, 4], [3, 3, 3], [1, 1, 2], [2, 1, 1]) ➞ 63

totalVolume([2, 2, 2], [2, 1, 1]) ➞ 10

totalVolume([1, 1, 1]) ➞ 1
```
### :sparkler:My Code
```js
function totalVolume(...boxes) {
   let arr = [...boxes].map((num) => {
      return num.reduce((prev, current) => {
        prev *= current;
        return prev;      
      })
    }) 
    return arr.reduce((prev, current) => prev+= current);
}
```
