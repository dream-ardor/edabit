## Array Multiplier

Create a function that takes an array as an argument and returns a new nested array for each element in the original array. The nested array must be filled with the corresponding element (string or number) in the original array and each nested array has the same amount of elements as the original array.
```js
Examples
multiply([4, 5]) ➞ [[4, 4], [5, 5]]

multiply(["*", "%", "$"]) ➞ [["*", "*", "*"], ["%", "%", "%"], ["$", "$", "$"]]

multiply(["A", "B", "C", "D", "E"]) ➞ [["A", "A", "A", "A", "A"], ["B", "B", "B", "B", "B"], ["C", "C", "C", "C", "C"], ["D", "D", "D", "D", "D"], ["E", "E", "E", "E", "E"]]

Notes
The given array contains numbers or strings.
```
### :sunny: My Code
```js
const multiply = a => a.map(b => Array.from({ length: a.length },() => b));


//alternate solutions
const multiply = a => a.map(l => a.map(r => l));

const multiply = arr => arr.map(i => Array(arr.length).fill(i));

const multiply = arr => arr.map(v => Array.from({length: arr.length}, _ => v));

```
