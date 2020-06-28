## RegEx XIX : Group Ranges - Capturing groups (x)

Groups and ranges indicate groups and ranges of expression characters. Capturing groups matches x in (x) and remembers the match.

"foo bar".match(/(foo)/) ➞ matches and remembers "foo"
Capturing groups often are used along with quantifiers. Quantifiers will use the capturing group as a whole.

"Gogogo now!".match(/(go)+/i) ➞ "Gogogo"
Caveat: Capturing groups have a performance penalty. If you don't need the matched substring to be recalled, prefer non-capturing parentheses.

MAC-address of a network interface consists of 6 two-digit hex numbers separated by a colon (e.g. 01:32:54:67:89:AB). Write a RegExp that checks whether a string is MAC-address.
```js
let regexp = /your regexp/

regexp.test("01:32:54:67:89:AB") ➞ true
regexp.test("0132546789AB") ➞ false
```
### :sunny: My Code
```js
const REGEXP = /^[\da-fA-F]{2}(:[\da-fA-F]{2}){5}$/i

//alternate
const REGEXP = /(\d+:){5}[^z]/i
```
