## Case Insensitive Comparison

Write a function that validates whether two strings are identical. Make this validator case insensitive.
```js
Examples
match("hello", "hELLo") ➞ true

match("motive", "emotive") ➞ false

match("venom", "VENOM") ➞ true

match("mask", "mAskinG") ➞ false
```
## 🆑 My Code
```js
const match = (a,b) => a.toUpperCase() == b.toUpperCase();
```
