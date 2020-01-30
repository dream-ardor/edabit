## Free Coffee Cups

Per 6 coffee cups I buy, I get a 7th cup free. In total, I get 7 cups. Create a function that takes n cups bought and return as an integer the total number of cups I would get.
```js
Examples
totalCups(6) ➞ 7

totalCups(12) ➞ 14

totalCups(213) ➞ 248
```
### :computer: My Code
```js
const totalCups = n => n + Math.floor(n / 6);
```
