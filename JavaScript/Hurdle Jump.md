## Hurdle Jump

Create a function that takes an array of hurdle heights and a jumper's jump height, and determine whether or not the hurdler can clear all the hurdles.

A hurdler can clear a hurdle if their jump height is greater than or equal to the hurdle height.
```js
Examples
hurdleJump([1, 2, 3, 4, 5], 5) ➞ true

hurdleJump([5, 5, 3, 4, 5], 3) ➞ false

hurdleJump([5, 4, 5, 6], 10) ➞ true

hurdleJump([1, 2, 1], 1) ➞ false
```

## Solution
```js
//Using Math.max
const hurdleJump = (hurdles, jumpHeight) => Math.max(...hurdles) <= jumpHeight

//Using .every()
const hurdleJump = (hurdles, jumpHeight) => hurdles.every (x => x <= jumpHeight)

//A traditional for loop
function hurdleJump(hurdles, jumpHeight) {
  for (var i in hurdles) {
  if (hurdles[i] > jumpHeight) 
  return false;
  }
  return true;
}
```
