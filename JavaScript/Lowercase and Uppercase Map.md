## Lowercase and Uppercase Map

Write a function that creates an object with each (key, value) pair being the (lower case, upper case) versions of a letter, respectively.
```js
Examples
mapping(["p", "s"]) ➞ { "p": "P", "s": "S" }

mapping(["a", "b", "c"]) ➞ { "a": "A", "b": "B", "c": "C" }

mapping(["a", "v", "y", "z"]) ➞ { "a": "A", "v": "V", "y": "Y", "z": "Z" }
```
### :leaves: My Code
```js
const mapping = l => Object.fromEntries(l.map(a=>[a, a.toUpperCase()]));
```
