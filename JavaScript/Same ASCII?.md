## Same ASCII?
Return true if the sum of ASCII values of the first string is same as the sum of ASCII values of the second string, otherwise return false.
```js
Examples
sameAscii("a", "a") ➞ true

sameAscii("AA", "B@") ➞ true

sameAscii("EdAbIt", "EDABIT") ➞ false
```
### :red_circle:My Code
```js
const sameAscii = (a, b) =>
a.split('').map(i => i.charCodeAt()).reduce((x,y) => x+y)
===
b.split('').map(i => i.charCodeAt()).reduce((x,y) => x+y)
```
