## Check if a String Contains only Identical Characters

Write a function that returns true if all characters in a string are identical and false otherwise.
```js
Examples
isIdentical("aaaaaa") ➞ true

isIdentical("aabaaa") ➞ false

isIdentical("ccccca") ➞ false

isIdentical("kk") ➞ true
```

## My Code
```js
const isIdentical = s => s.split('').every(x => x === s[0]);

//Here is a solution using regex
const isIdentical = s => /^(.)\1*$/.test(s);

```
