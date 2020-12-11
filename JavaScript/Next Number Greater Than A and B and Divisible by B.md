## Next Number Greater Than A and B and Divisible by B

You are given two numbers a and b. Create a function that returns the next number greater than a and b and divisible by b.
```js
Examples

divisibleByB(17, 8) ➞ 24

divisibleByB(98, 3) ➞ 99

divisibleByB(14, 11) ➞ 22
```
### :leaves: My Code
```js
let divisibleByB = (a,b) => b * Math.ceil(a/b);

//alternate solution
const divisibleByB = (a, b) => {
  let c = a + 1;
  while( c % b != 0) {c += 1};
  return c;
}
```
