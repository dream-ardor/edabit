## Online Shopping
Create a function that determines whether a shopping order is eligible for free shipping. An order is eligible for free shipping if the total cost of items purchased exceeds $50.00.
```js
Examples
freeShipping({ "Shampoo": 5.99, "Rubber Ducks": 15.99 }) ➞ false

freeShipping({ "Flatscreen TV": 399.99 }) ➞ true

freeShipping({ "Monopoly": 11.99, "Secret Hitler": 35.99, "Bananagrams"
```
### :kaaba: My Code
```js
function freeShipping(o) {
  let a = Object.keys(o).reduce((a,b)=>a+parseFloat(o[b]||0),0);
  return a > 50;
}
```
