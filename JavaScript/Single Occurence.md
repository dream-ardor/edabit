## Single Occurrence

Create a function that, given a string str, finds a letter that has a single occurrence. Return the letter in uppercase. If the input is empty, return an empty string "".
```js
Examples
singleOccurrence("EFFEAABbc") ➞ "C"

singleOccurrence("AAAAVNNNNSS") ➞ "V"

singleOccurrence("S") ➞ "S"
```
### :palm_tree: My Code
```js
const singleOccurrence = s => s.toUpperCase().split('').sort().join('').replace(/(\w)\1+/g,'').slice(0,1);
```
