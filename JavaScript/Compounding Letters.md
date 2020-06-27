## Compounding Letters

Create a function that takes a string and returns a new string with each new character accumulating by +1. Separate each set with a dash.
```js
Examples
accum("abcd") ➞ "A-Bb-Ccc-Dddd"

accum("RqaEzty") ➞ "R-Qq-Aaa-Eeee-Zzzzz-Tttttt-Yyyyyyy"

accum("cwAt") ➞ "C-Ww-Aaa-Tttt"
```
### My Code
```js
const accum = s => [...s].map((a,b)=> a.toUpperCase() + a.toLowerCase().repeat(b)).join('-');
```
