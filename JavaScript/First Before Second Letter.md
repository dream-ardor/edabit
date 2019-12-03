## First Before Second Letter

You are given three inputs: a string, one letter, and a second letter.

Write a function that returns true if every instance of the first letter occurs before every instance of the second letter.
```js
Examples
firstBeforeSecond("a rabbit jumps joyfully", "a", "j") ➞ true
// every instance of "a" occurs before every instance of "j"

firstBeforeSecond("knaves knew about waterfalls", "k", "w") ➞  true

firstBeforeSecond("happy birthday", "a", "y") ➞ false
// the "a" in "birthday" occurs after the "y" in "happy"

firstBeforeSecond("precarious kangaroos", "k", "a") ➞ false
```
### :maple_leaf: My Code
```js
let firstBeforeSecond = (s, f, se) =>
  s.indexOf(se) >= s.lastIndexOf(f);
```