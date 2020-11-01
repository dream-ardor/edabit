## Is the Water Boiling?

Create a function that determines if the temp of the water is considered boiling or not. temp will be measured in fahrenheit and celsius.
```js
Examples
isBoiling("212F") ➞ true

isBoiling("100C") ➞ true

isBoiling("0F") ➞ false

Notes:
The boiling point of water is 212F in fahrenheit and 100C in celsius.
```
### :jack_o_lantern: My Code
```js
const isBoiling = t => t.match(/\d/g).join('') >= 100; 
```
