## How Many Decimal Places?

Create a function that returns the number of decimal places a number (given as a string) has. Any zeros after the decimal point count towards the number of decimal places.
```js
Examples
getDecimalPlaces("43.20") ➞ 2

getDecimalPlaces("400") ➞ 0

getDecimalPlaces("3.1") ➞ 1
```
### :leaves: My Code
```js
const getDecimalPlaces = n => 
 n.includes('.') ? n.split('.')[1].length : 0;
```
