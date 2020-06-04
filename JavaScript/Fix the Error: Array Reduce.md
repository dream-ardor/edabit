## Fix The Error: Array Reduce

The instructor assigns Boron two tasks (regarding the use of reduce() method after lecturing in array methods).

The first task is to create a function calculateSum() that takes a string and returns the sum of the ASCII values of all the characters in the string using reduce().
The second task is to create a function reverseString() that reverses and returns an input string using reduce().
While solving the problem, Boron has encountered errors. Help him fix the errors.
```js
Examples
calculateSum("lime") ➞ 423
// 108 + 105 + 109 + 101 = 423

calculateSum("a") ➞ 97
// a = 97

reverseString("hello") ➞ "olleh"
```
### :computer: My Code
```js
const calculateSum = a =>
 [...a].reduce((b,c)=>b + c.charCodeAt(),0);

const reverseString = b => [...b].reduce((a, b)=> b+a,'');

```
