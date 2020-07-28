## First N Mid

Create a function that takes a string and returns the first character of every word if the length is even and the middle character if the length is odd.
```js
Examples
stmid("Alexa have to paid") ➞ "ehtp"

stmid("Th3 0n3 4nd 0n1y") ➞ "hnn0"

stmid("who is the winner") ➞ "hihw"
```
### :computer: My Code
```js
const stmid = str => str.split(" ").map(w => w[(l = w.length) % 2 && l / 2 | 0]).join("");

//alternate
const stmid = s => s.split(' ').map(v => v[v.length % 2 ? v.length >> 1 : 0]).join('');
```
