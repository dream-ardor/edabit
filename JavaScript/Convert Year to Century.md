## Convert Year to Century

Write a function that takes a year and returns its corresponding century.
```js
Examples
centuryFromYear(2005) ➞ 21

centuryFromYear(1950) ➞ 20

centuryFromYear(1900) ➞ 19
```
### :computer: My Code
```js
const centuryFromYear = y => Math.ceil(y/100);
```
