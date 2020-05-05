## Change Every Letter to the Next Letter

Write a function that changes every letter to the next letter:
```js
"a" becomes "b"
"b" becomes "c"
"d" becomes "e"
and so on ...

Examples
move("hello") ➞ "ifmmp"

move("bye") ➞ "czf"

move("welcome") ➞ "xfmdpnf"
```
### :leaves: My Code
```js
const move = w => 
 [...w].map(b => String.fromCharCode(b.charCodeAt() + 1)).join('');
```
