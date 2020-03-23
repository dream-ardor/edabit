## Check If Lines Are Parallel

Given two lines, determine whether or not they are parallel.

Lines are represented by an array [a, b, c], which corresponds to the line ax+by=c.
```js
Examples
linesAreParallel([1, 2, 3], [1, 2, 4]) ➞ true
// x+2y=3 and x+2y=4 are parallel.

linesAreParallel([2, 4, 1], [4, 2, 1]) ➞ false
// 2x+4y=1 and 4x+2y=1 are not parallel.

linesAreParallel([0, 1, 5], [0, 1, 5]) ➞ true
// Lines are parallel to themselves.
```
### :computer: My Code
```js
const linesAreParallel = (l1, l2) => l1[0]/l1[1] == l2[0]/l2[1];

//alternate
const linesAreParallel = ([a, b, c], [x, y, z]) =>  a/b === x/y
```
