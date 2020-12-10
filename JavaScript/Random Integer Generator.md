## Random Integer Generator

The challange is simple. Return a random integer N such that a <= N <= b.
```js
Examples
randomInt(5, 9) ➞ 7

randomInt(5, 9) ➞ 9

randomInt(5, 9) ➞ 5
```
### :palm_tree: My Code
```js
const randomInt = (a,b) => ~~(Math.random()*(b-a) + a);


//alternate solution
const randomInt = (a,b) => Math.floor(Math.random() * (b-a)) + a;
```
