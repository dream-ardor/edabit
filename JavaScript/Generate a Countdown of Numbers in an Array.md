## Generate a Countdown of Numbers in an Array

Create a function that takes a number as an argument and returns an array of numbers counting down from this number to zero.
```js
Examples
countdown(5) ➞ [5, 4, 3, 2, 1, 0]

countdown(1) ➞ [1, 0]

countdown(0) ➞ [0]
```

## My Code
```js
//Using a for loop

let countdown = start => {
	let s = [];
	for (let i = start; i >= 0; i--) {
		s.push(i);
	}
	return s;
}

//Object.keys() and reverse method

const countdown = start => [...Array(start + 1).keys()].reverse();


//Another way to do it by using Array.from

function countdown(start) {
	return Array.from({length: start + 1}, (_,i) => start - i)
}

```
