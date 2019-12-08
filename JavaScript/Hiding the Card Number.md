## Hiding the Card Number

Write a function that takes a credit card number and only displays the last four characters. The rest of the card number must be replaced by ************.
```js
Examples
cardHide("1234123456785678") ➞ "************5678"

cardHide("8754456321113213") ➞ "************3213"

cardHide("35123413355523") ➞ "**********5523"
```
## :maple_leaf: My Code
```js
let cardHide = c => c.slice(-4).padStart(c.length,'*');
```
