## Return the Remainder from Two Numbers

There is a single operator in JavaScript capable of providing the remainder of a division operation. Two numbers are passed as parameters. The first provider divided by the second parameter will have a remainder, possiby zero. Return that value.
```js
Examples

remainder(1, 3) ➞ 1

remainder(-9, 45) ➞ -9

remainder(5, 5) ➞ 0
```

## My Code
```js
function remainder(x, y) {
	return x % y;
}
```

## Analysis
Using the modulus operator returns the remainder.
