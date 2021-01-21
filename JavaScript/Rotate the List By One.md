## Rotate the List by One 🔄

Given a list, rotates the values clockwise by one (the last value is sent to the first position).

Check the examples for a better understanding.
```js
Examples
rotate_by_one([1, 2, 3, 4, 5]) ➞ [5, 1, 2, 3, 4]

rotate_by_one([6, 5, 8, 9, 7]) ➞ [7, 6, 5, 8, 9]

rotate_by_one([20, 15, 26, 8, 4]) ➞ [4, 20, 15, 26, 8]
```
### :us: My Code
```js
const rotateByOne = a => (a.unshift(a.pop()),a);


//alternate solution
const rotateByOne = a => a.slice(-1).concat(a.slice(0,-1));
```
