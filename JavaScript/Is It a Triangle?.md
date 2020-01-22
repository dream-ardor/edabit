## Is It a Triangle?

Create a function that takes three numbers as arguments and returns true if it's a triangle and false if not.
```js
Examples
isTriangle(2, 3, 4) ➞ true

isTriangle(3, 4, 5) ➞ true
```
### :evergreen_tree: My Code
```js
const isTriangle = (a, b, c) =>
 (a+b) > c && (b+c) > a && (a+c) > b;
```
