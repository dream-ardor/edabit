## Is the String in Order?
Create a function that takes a string and returns true or false, depending on whether the characters are in order or not.
```js
Examples
isInOrder("abc") ➞ true

isInOrder("edabit") ➞ false

isInOrder("123") ➞ true

isInOrder("xyzz") ➞ true
```
### :fork_and_knife: My Code
```js
const isInOrder = s =>  s == [...s].sort().join('');
```
