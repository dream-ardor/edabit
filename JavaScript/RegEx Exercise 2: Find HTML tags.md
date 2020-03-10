## RegEx Exercise 2: Find HTML tags
```js
Challenge:
Create a regular expression to find all (opening and closing) HTML tags with their attributes
Assume that tag attributes may not contain < and > (inside quotes too)
const REGEXP = /your regexp/g;

let str = '<> <a href="/"> <input type="radio" checked> <b>';

str.match(REGEXP) ➞  '<a href="/">', '<input type="radio" checked>', '<b>'
```
### :computer: My Code
```js
const REGEXP = /<[^<>]+>/g
```
