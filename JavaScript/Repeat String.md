## Repeat String
Create a function that takes a string txt and a number n and returns the repeated string n number of times.

If given argument txt is not a string, return Not A String !!
```js
Examples
repeatString("Mubashir", 2) ➞ "MubashirMubashir"

repeatString("Matt", 3) ➞ "MattMattMatt"

repeatString(1990, 7) ➞ "Not A String !!"
```
### :leaves: My Code
```js
const repeatString = (t,n) => String(t) === t ? t.repeat(n) : "Not A String !!";
```
