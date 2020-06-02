## Is it a Valid Floating Numeric Character?

Create a regular expression to check whether the given string is a valid floating numeric character or not.
```js
Examples
isFloatingCharacter("12.12") ➞ true

isFloatingCharacter("12.") ➞ false

isFloatingCharacter(".1") ➞ true

isFloatingCharacter("-.1") ➞ true

isFloatingCharacter("abc") ➞ false
```
### :computer: My Code
```js
const isFloatingCharacter = n =>/^-?\d*\.\d+$/.test(n);                               
```
