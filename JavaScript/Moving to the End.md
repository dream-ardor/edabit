## Moving to the End

Write a function that moves all elements of one type to the end of the array.
```js
Examples
moveToEnd([1, 3, 2, 4, 4, 1], 1) ➞ [3, 2, 4, 4, 1, 1]
// Move all the 1s to the end of the array.

moveToEnd([7, 8, 9, 1, 2, 3, 4], 9) ➞ [7, 8, 1, 2, 3, 4, 9]

moveToEnd(["a", "a", "a", "b"], "a") ➞ ["b", "a", "a", "a"]
```
### :computer: My Code
```js
const moveToEnd = (a,e) => a.filter(x => x !== e).concat(a.filter(x => x == e));
 
 //alternate
 const moveToEnd = (a, el) => a.sort(x => x == el ? 1 : 0);
```
