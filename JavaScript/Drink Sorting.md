## Drink Sorting

You will be given an array of drinks, with each drink being an object with two properties: name and price. Create a function that has the drinks array as an argument and return the drinks object sorted by price in ascending order.

Assume that the following array of drink objects needs to be sorted:
```js
drinks = [
    {name: 'lemonade', price: 50},
    {name: 'lime', price: 10}
];
```
The output of the sorted drinks object will be:
```js
Examples
sortDrinkByPrice(drinks) ➞ [{name: 'lime', price: 10}, {name: 'lemonade', price: 50}]
```
### :champagne: My Code
```js
const sortDrinkByPrice = d => 
 d.sort((a,b)=> a.price - b.price);
```
