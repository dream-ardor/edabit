## Tuck In Array

Insert an array into another array

Create a function that takes two arrays as argument and insert the second array in the middle of the first array
Use the spread syntax to solve this challenge.
Try to type your code after the return statement and solve the challenge in one line.
```
[1,10], [2,3,4,5,6,7,8,9] ➞  [1,2,3,4,5,6,7,8,9,10]

[15,150], [45, 75, 35] ➞  [15, 45, 75, 35, 150]
*array1 has always just 2 elements
```
### :sunny: My Code
```js
const tuckIn = (a,b) => [a[0],...b,a.pop()];
```
