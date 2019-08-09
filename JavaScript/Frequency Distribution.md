## Frequency Distribution
Create a function that returns the frequency distribution of an array. This function should return an object, where the keys are the unique elements and the values are the frequency in which those elements occur.
```js
Examples
getFrequencies(["A", "B", "A", "A", "A"]) ➞ { A: 4, B: 1 }

getFrequencies([1, 2, 3, 3, 2]) ➞ { "1": 1, "2": 2, "3": 2 }

getFrequencies([true, false, true, false, false]) ➞ { true: 2, false: 3 }

getFrequencies([]) ➞ {}
```
### :key:My Code
```js
//using Object.assign
const getFrequencies = arr => 
arr.reduce((x,y) =>
	Object.assign(x, x[y] ? x[y]++ : (x[y] = 1)), {});
	
//using Map
const getFrequencies = arr => {
	let a = {};
	arr.map(x => a[x] = a[x] + 1 || 1)
	return a;
}
```
