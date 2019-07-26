## H4ck3r Sp34k
Create a function that takes a string as an argument and returns a coded (h4ck3r 5p34k) version of the string.
```js
Examples
hackerSpeak("javascript is cool") ➞ "j4v45cr1pt 15 c00l"

hackerSpeak("programming is fun") ➞ "pr0gr4mm1ng 15 fun"

hackerSpeak("become a coder") ➞ "b3c0m3 4 c0d3r"
```

### :computer: My Code
```js
const hackerSpeak = str => str.replace(/a/g, 4).replace(/e/g,3).replace(/i/g,1)
.replace(/o/g,0).replace(/s/g,5);
```
