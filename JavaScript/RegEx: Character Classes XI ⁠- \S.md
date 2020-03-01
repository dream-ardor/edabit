## RegEx: Character Classes XI ⁠- \S

You can think of character classes as characters with special meaning. They are recognized as special when you place the \ before the character.

Here are a list of the characters classes in JavaScript:
```js
., \cX, \d, \D, \f, \n, \r, \s, \S, \t, \v, \w, \W, \0, \xhh, \uhhhh, \uhhhhh, [\b]
```
Write a regex that will return true if the bio does not have any spaces before the last ending punctuation ?. You must use the \S character class in your expression.
### :computer: My Code
```js
const REGEXP = /\S\?/g

//alternate
const REGEXP = /\S[?]/g
```
