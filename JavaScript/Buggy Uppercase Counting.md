## Buggy Uppercase Counting

In the Code tab is a function which is meant to return how many uppercase letters there are in a list of various words. Fix the list comprehension so that the code functions normally!
```
Examples

countUppercase(["SOLO", "hello", "Tea", "wHat"]) ➞ 6

countUppercase(["little", "lower", "down"]) ➞ 0

counUppercase(["EDAbit", "Educate", "Coding"]) ➞ 5
```
### :palm_tree: My Code
```js
const countUppercase = s => (s.join('').match(/[A-Z]/g) || []).length;
```
