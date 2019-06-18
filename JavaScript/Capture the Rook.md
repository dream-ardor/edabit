## Capture the Rook

Write a function that returns true if two rooks can attack each other, and false otherwise.
```js
Examples
canCapture(["A8", "E8"]) ➞ true

canCapture(["A1", "B2"]) ➞ false

canCapture(["H4", "H3"]) ➞ true

canCapture(["F5", "C8"]) ➞ false
```

## My Code
```js
const canCapture = ([yourRook, opponentsRook]) => 
yourRook.charAt(0) == opponentsRook.charAt(0)
||
yourRook.slice(-1) == opponentsRook.slice(-1)

```
