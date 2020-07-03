## Friday the 13th

Given the month and year as numbers, return whether that month contains a Friday 13th.
```js
Examples
hasFriday13(3, 2020) ➞ true

hasFriday13(10, 2017) ➞ true

hasFriday13(1, 1985) ➞ false
```
### :computer: My Code
```js
const hasFriday13 = (m,y) => new Date(y, m-1, 13).getDay() == 5;
```
