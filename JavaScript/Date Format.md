## Date Format
Create a function that converts a date formatted as MM/DD/YYYY to a format required as YYYYDDMM. The parameter userDate and the return value are strings.
```js
Examples
formatDate("11/12/2019") ➞ "20191211"

formatDate("12/31/2019") ➞ "20193112"
```
### :fallen_leaf: My Code
```js
let formatDate = u => u.split('/').reverse().join('');

```
