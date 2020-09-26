## Recreating the String.length Property

Create a function which returns the length of a string, WITHOUT using String.length property.
```js
Examples
length("Hello World") ➞ 11

length("Edabit") ➞ 6

length("wash your hands!") ➞ 16
```
### :computer: My Code
```js
const length = s => [...s].reduce(a => a+1, 0);
```
