## Does the Object Contain a Given Key?
Write a function that returns true if a hash contains the specified key, and false otherwise.
```js
Examples
hasKey({ a: 44, b: 45, c: 46 }, "d") ➞ false

hasKey({ craves: true, midnight: true, snack: true }, "morning") ➞ false

hasKey({ pot: 1, tot: 2, not: 3 }, "not") ➞ true
```
### :jack_o_lantern: My Code
```js
const hasKey= (o, k) => o.hasOwnProperty(k);
```
