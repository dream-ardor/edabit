## Alphanumeric Restriction

Create a function that returns true if the given string has any of the following:
```
Only letters and no numbers.
Only numbers and no letters.
```
If a string has both numbers and letters, or contains characters which don't fit into any category, return false
```js
Examples
alphanumericRestriction("Bold") ➞ true

alphanumericRestriction("123454321") ➞ true

alphanumericRestriction("H3LL0") ➞ false

alphanumericRestriction("ed@bit") ➞ false

Notes
Any string that contains spaces or is empty should return false.
```
### :computer: My Code
```js
const alphanumericRestriction = s =>
 /^[a-z]+$/i.test(s) || /^[\d]+$/.test(s);
```
