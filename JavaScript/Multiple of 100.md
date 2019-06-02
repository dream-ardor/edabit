## Multiple of 100

Create a function that takes an integer and returns true if it's divisible by 100, otherwise return false.
```js
Examples
divisible(1) ➞ false

divisible(1000) ➞ true

divisible(100) ➞ true
```

## My Code
```js
function divisible(num) {
	if (num % 100 === 0) {
		return true;
	}
	else {
		return false;
	}
}
```
