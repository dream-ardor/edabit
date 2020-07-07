## In the Centre?

Given a string containing mostly spaces and one non-space character, return whether the character is positioned in the very centre of the string. This means the number of spaces on both sides should be the same.
```js
Examples
isCentral("  #  ") ➞ true

isCentral(" 2    ") ➞ false

isCentral("@") ➞ true
```
### :computer: My Code
```js
let isCentral = s => s.trimStart().length == s.trimEnd().length;
```
