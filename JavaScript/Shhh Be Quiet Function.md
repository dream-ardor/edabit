## Shhh Be Quiet Function

Write a function that removes all capitals letters from a sentence except the first letter, put quotation marks around the sentence and add ", whispered Edabit." to the end.
```js
Examples
shhh("HI THERE!") ➞ '"Hi there!", whispered Edabit.'

shhh("tHaT'S Pretty awesOme") ➞ '"That's pretty awesome", whispered Edabit.'

shhh("") ➞ '"", whispered Edabit.'
```
### :computer: My Code
```js
const shhh = s => `"${s.charAt(0).toUpperCase()}${s.slice(1).toLowerCase()}", whispered Edabit.`;
```
