## RegEx: Special Characters

Using the test method in your function, return whether a string contains the characters a and c (in that order) with any number of b characters (including zero) between them.
```js
Examples
asterisk("account") ➞ true

asterisk("abccount") ➞ true

asterisk("abbbccount") ➞ true

asterisk("bbbccount") ➞ false
```
### :football: My Code
```js
const asterisk = s => /ab*c/.test(s);
```
