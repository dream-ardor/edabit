## Jay and Silent Bob Weight Convertor

Jay and Silent Bob have been given a fraction of an ounce but they only understand grams. Convert a fraction passed as a string to grams with up to two decimal places. An ounce weighs 28 grams.
```js
Examples
jayAndBob("half") ➞ "14 grams"

jayAndBob("quarter") ➞ "7 grams"

jayAndBob("eighth") ➞ "3.5 grams"

Notes
Add the string "grams" to the end with a space.
```
### :palm_tree: My Code
```js
const jayAndBob = s => {
 let a = {
  "half":"14 grams",
  "quarter":"7 grams",
  "eighth":"3.5 grams",
  "sixteenth": "1.75 grams"
  }
  return a[s];
}


//alternate solutions
const jayAndBob = s => `${s == 'half' ? 14 : s == 'quarter' ? 7 : s == 'eighth' ? 3.5 : 1.75} grams`;


function jayAndBob(str) {
  return {
   half: "14 grams",
   quarter: "7 grams",
   eighth : "3.5 grams",
   sixteenth: "1.75 grams"
  }[str];
}

```
