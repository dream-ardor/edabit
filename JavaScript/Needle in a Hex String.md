## Needle in a Hex String

Find the index of a string within a hex encoded string.

You will be given a string which needs to be found in another string which has previously been translated into hex. You will need to return the first index of the needle within the hex encoded string.
```js
Examples
firstIndex("68 65 6c 6c 6f 20 77 6f 72 6c 64", "world") ➞ 6

firstIndex("47 6f 6f 64 62 79 65 20 77 6f 72 6c 64", "world") ➞ 8

firstIndex("42 6f 72 65 64 20 77 6f 72 6c 64", "Bored") ➞ 0
```
### :computer: My Code
```js
const firstIndex = (h, n) => 
 h.indexOf(n.split("")
 .map(char => char.charCodeAt().toString(16))
 .join(" ")) / 3;

```
