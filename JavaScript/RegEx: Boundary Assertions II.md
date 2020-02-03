## RegEx: Boundary Assertions II

You are give an array with random words but your program doesn't accept words that begin with the capital letter "C". Remove the unaccepted words and return the new array.
```js
Examples
accepted(["Ducks", "Bears",  "Cats"]) ➞ ["Ducks", "Bears"]

accepted(["cars", "trucks", "planes"] ➞ ["cars", trucks", "planes"]

accepted(["Cans", "Worms", "Bugs", "Cold", "Beans"]) ➞ ["Worms", "Bugs", "Beans"]
```

### :football: My Code
```js

const acceptedWords = a => a.filter(x => x.replace(/\bC+\S+/g, ''));

//alternate regex
const acceptedWords = arr => arr.filter(v => !/^C/.test(v));

```
