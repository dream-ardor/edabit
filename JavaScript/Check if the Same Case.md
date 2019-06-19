## Check if the Same Case

Create a function that returns true if an input string contains only uppercase or only lowercase letters.
```js
Examples:
sameCase("hello") ➞ true

sameCase("HELLO") ➞ true

sameCase("Hello") ➞ false

sameCase("ketcHUp") ➞ false
```

## My Code
```js
const sameCase = str => str == str.toLowerCase() || str == str.toUpperCase();

//Using Regex
const sameCase = str => /^[A-Z]*$/.test(str) || /^[a-z]*$/.test(str);
```
