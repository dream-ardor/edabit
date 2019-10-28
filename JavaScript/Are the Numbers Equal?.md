## Are the Numbers Equal?
Create a function that takes two integers and checks if they are equal.
```js
Examples
isEqual(5, 6) ➞ false

isEqual(1, 1) ➞ true

isEqual("1", 1) ➞ false
```
### :jack_o_lantern: My Code
```js
const isEqual = (n1, n2) => typeof n1 == 'string' ? false : n1 === n2;
```
