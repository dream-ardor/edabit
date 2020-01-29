## Profit Margin

Create a function that calculates the profit margin given costPrice and salesPrice. Return the result as a percentage formated string, and rounded to one decimals. To calculate profit margin you subtract the cost from the sales price, then divide by salesprice.
```js
Examples
profitMargin(50, 50) ➞ "0.0%"

profitMargin(28, 39) ➞ "28.2%"

profitMargin(33, 84) ➞ "60.7%"
```
### :dollar: My Code
```js
const profitMargin = (c, s) => 
 (((s - c) / s) * 100).toFixed(1) + '%';
```
