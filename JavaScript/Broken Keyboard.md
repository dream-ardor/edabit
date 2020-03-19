## Broken Keyboard

Given what is supposed to be typed and what is actually typed, write a function that returns the broken key(s). The function looks like:
```js
findBrokenKeys(correct phrase, what you actually typed)

Examples:
findBrokenKeys("happy birthday", "hawwy birthday") ➞ ["p"]

findBrokenKeys("starry night", "starrq light") ➞ ["y", "n"]

findBrokenKeys("beethoven", "affthoif5") ➞ ["b", "e", "v", "n"]

Notes:
- Broken keys should be ordered by when they first appear in the sentence.
- Only one broken key per letter should be listed.
- Letters will all be in lower case.
```
### :computer: My Code
```js
const findBrokenKeys = (s1, s2) =>
 [...new Set([...s1+''].filter((a,b)=> a !== s2[b]))];
```
