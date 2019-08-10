## Switcharoo
Create a function that takes a string and returns a new string with its first and last characters swapped, except under three conditions:
```
If the length of the string is less than two, return "Incompatible.".
If the argument is not a string, return "Incompatible.".
If the first and last characters are the same, return "Two's a pair.".
```
```js
Examples
flipEndChars("Cat, dog, and mouse.") ➞ ".at, dog, and mouseC"

flipEndChars("ada") ➞ "Two's a pair."

flipEndChars("Ada") ➞ "adA"

flipEndChars("z") ➞ "Incompatible."

flipEndChars([1, 2, 3]) ➞ "Incompatible."
```
### :musical_keyboard:My Code
```js
const flipEndChars = str => 
 typeof str !== "string" || str.length < 2 ? "Incompatible.":
  str[0] === str[str.length-1] ? "Two's a pair." : 
  `${str[str.length-1]}${str.substring(1,str.length-1)}${str[0]}`;
```
