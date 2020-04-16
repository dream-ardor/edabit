## One Button Messaging Device

Imagine a messaging device with only one button. For the letter A, you press the button one time, for E, you press it five times, for G, it's pressed seven times, etc, etc.

Write a function that takes a string (the message) and returns the total number of times the button is pressed.
```js
Examples
howManyTimes("abde") ➞ 12

howManyTimes("azy") ➞ 52

howManyTimes("qudusayo") ➞ 123
```
### :computer: My Code
```js
const howManyTimes = m => [...m].reduce((a,b) => a + b.charCodeAt()-96, 0);
```
