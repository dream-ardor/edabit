## Rotate Max Number

Create a function which takes a number and returns the maximum value by rearranging its digits.
```js
Examples
rotateMaxNumber(123) ➞ 321

rotateMaxNumber("001") ➞ 100

rotateMaxNumber(999) ➞ 999
```
### :leaves: My Code
```js
const rotateMaxNumber = n => +[...n+''].sort((a,b)=> b - a).join('');


//alternate solution
const rotateMaxNumber = n => +([...n+''].sort().reverse().join(''));
```
