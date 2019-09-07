## Is Sam with Frodo?
Sam and Frodo need to be close. If they are side by side in the array, your function should return true. If there is a name between them, return false.
```js
Examples
middleEarth(["Frodo", "Sam", "Gandalf"]) ➞ true

middleEarth(["Frodo", "Saruman", "Sam"]) ➞ false

middleEarth(["Orc", "Sam", "Frodo", "Legolas"]) ➞ true
```
### :kaaba: My Code
```js
const middleEarth = a =>
 Math.abs(a.indexOf('Sam') - a.indexOf('Frodo')) === 1 
```
