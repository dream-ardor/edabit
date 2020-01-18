## Last Character of First Name

Create a function that takes a string as an argument. The string is a random name.

If the last character of the name is an "n", return true.
If the last character of the name is not an "n", return false.
```js
Examples
isLastCharacterN("Aiden") ➞ true

isLastCharacterN("Piet")  ➞ false
```

### :evergreen_tree: My Code
```js
let isLastCharacterN = w => w.endsWith('n');
```
