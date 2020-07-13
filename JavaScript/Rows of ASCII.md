## Rows of ASCII

Given a very long string of ASCII characters, split the string up into equal sized groups of size width. To properly display the image, join up the groups with the newline character \n and return the output string.

See the following examples for clarity!
```js
Examples
formatAscii('0123456789', 2) ➞ '01\n23\n45\n67\n89'

formatAscii('................................', 8) ➞ '........\n........\n........\n........'

formatAscii('^^^^^^^^', 1) ➞ '^\n^\n^\n^\n^\n^\n^\n^'
```
### :sunny: My Code
```js
const formatAscii = (s, w) => s.match(new RegExp(`.{${w}}`, 'g')).join('\n');
```
