## On the Nth Day of Christmas...

Throughout the 12 days of Christmas, my true love gave me in total 364 items.

Create a function where given n days as an argument, return the total amount of items received throughout those days as an integer.
```js
Examples
xmasItems(12) ➞ 364

xmasItems(3) ➞ 10

xmasItems(31) ➞ 5456
```
### :herb: My Code
```js
const xmasItems = n => (n/6) * (n + 1) * (n + 2);
```
