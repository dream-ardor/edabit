The Reverser!
The "Reverser" takes a string as input and returns that string in reverse order, with the opposite case.
```js
Examples
reverse("Hello World") ➞ "DLROw OLLEh"

reverse("ReVeRsE") ➞ "eSrEvEr"

reverse("Radar") ➞ "RADAr"
```
### :computer: My Code
```js
const reverse = t => [...t].map((c) => c === c.toUpperCase() 
 ? c.toLowerCase() : c.toUpperCase()).reverse().join('')
```
