## Find Unique Character Strings
Create a function that returns only strings with unique characters.
```js
Examples
filterUnique(["abb", "abc", "abcdb", "aea", "bbb"]) ➞ ["abc"]
// "b" occurs in "abb" more than once, "b" occurs in "abcdb" more than once, etc.

filterUnique(["88", "999", "989", "9988", "9898"]) ➞ []

filterUnique(["ABCDE", "DDEB", "BED", "CCA", "BAC"]) ➞ ["ABCDE", "BED", "BAC"]
```
###  :leftwards_arrow_with_hook:My Code
```js
const filterUnique = arr => arr.filter(x => new Set(x).size === x.length);
```
