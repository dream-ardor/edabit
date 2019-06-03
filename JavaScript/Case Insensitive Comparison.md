## Case Insensitive Comparison

Write a function that validates whether two strings are identical. Make this validator case insensitive.
```js
Examples
match("hello", "hELLo") ➞ true

match("motive", "emotive") ➞ false

match("venom", "VENOM") ➞ true

match("mask", "mAskinG") ➞ false
```
## My Code
```js
function match(s1, s2) {
	if (s1.toUpperCase() === s2.toUpperCase()) {
	 return true;
	}
	else {
	 return false;
	}
}
```
