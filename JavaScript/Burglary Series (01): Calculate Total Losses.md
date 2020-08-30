## Burglary Series (01): Calculate Total Losses

You just returned home to find your mansion has been robbed! Given an object of the stolen items, return the total amount of the burglary (number). If nothing was robbed, return the string "Lucky you!".
```js
Examples
const stolenItems = {
  tv: 30,
  skate: 20,
  stereo: 50,
} ➞ 100

const stolenItems = {
  painting: 20000,
} ➞ 20000

const stolenItems = {} ➞ "Lucky you!"
```
```
Notes:
The item value is always positive.
```
### :leaves: My Code
```js
const calculateLosses = o => Object.values(o).reduce((a,b) => a+b, 0) || "Lucky you!";
```
