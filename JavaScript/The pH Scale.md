## The pH Scale

Given a pH value, return whether that value is 'alkaline', 'acidic', or 'neutral'. Return 'invalid' if the value given is less than 0 or greater than 14.
```js
Examples
pHName(5) ➞ "acidic"

pHName(8.7) ➞ "alkaline"

pHName(7) ➞ "neutral"
```
### :computer: My Code
```js
const pHName = p => p < 0 || p > 14 ? 'invalid' :
 p < 7 ? 'acidic' : p > 7 ? 'alkaline' : 'neutral';
```
