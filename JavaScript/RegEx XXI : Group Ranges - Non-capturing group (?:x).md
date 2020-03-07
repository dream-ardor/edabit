## RegEx XXI : Group Ranges - Non-capturing group (?:x)

Groups and ranges indicate groups and ranges of expression characters. Non-capturing groups matches "x" and behaves like capturing groups, but it does not remember the match.

Keep in mind that capturing groups have a performance penalty. If you don't need the matched substring to be recalled, prefer non-capturing groups
```js
Challenge

Write a regex that matches colors in the format #abc or #abcdef
That is: # followed by 3 or 6 hexadecimal digits.
Use a non capturing group in your expression
let REGEXP = /your regexp/g
let str = "color: #3f3; background-color: #AA00ef; and: #abcd"
str.match(REGEXP) ; ➞  #3f3 #AA00ef
```
### :leaves: My Code
```js
let REGEXP = /#(?:([a-f\d]{3}){1,2})\b/gi
```
