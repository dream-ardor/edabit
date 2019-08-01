## Count Ones in Binary Representation of Integer
Count the amount of ones in the binary representation of an integer. So for example, since 12 is '1100' in binary, the return value should be 2.
```js
Examples
countOnes(0) ➞ 0

countOnes(100) ➞ 3

countOnes(999) ➞ 8
```
### :eight_spoked_asterisk:My Code
```js
function countOnes(i) {
	let a = i.toString(2);
	return a.includes(1) ? a.match(/1/g).length : 0;
}
```
