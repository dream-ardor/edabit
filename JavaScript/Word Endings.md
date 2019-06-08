## Word Endings

Create a function that adds a string ending to each member in an array.
```js
Examples
addEnding(["clever", "meek", "hurried", "nice"], "ly")
➞ ["cleverly", "meekly", "hurriedly", "nicely"]

addEnding(["new", "pander", "scoop"], "er")
➞ ["newer", "panderer", "scooper"]

addEnding(["bend", "sharpen", "mean"], "ing")
➞ ["bending", "sharpening", "meaning"]
```

## My Code
```js
const addEnding = (arr, ending) => arr = arr.map(i => i + ending);

```
