## Reverse Coding Challenge #6
This is a reverse coding challenge. Normally you're given explicit directions with how to create a function. Here, you must generate your own function to satisfy the relationship between the inputs and outputs.

Your task is to create a function that, when fed the inputs below, produce the sample outputs shown.
```js
Examples
mysteryFunc(152) ➞ 10

mysteryFunc(832) ➞ 48

mysteryFunc(19) ➞ 9

mysteryFunc(133) ➞ 9
```
### :watch:My Code
```js
const mysteryFunc = num => num.toString().split('').reduce((a,b) => a * b);

```
