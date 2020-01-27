## Capitalize the Last Letter

Create a function that capitalizes the last letter of every word.
```js
Examples
capLast("hello") ➞ "hellO"

capLast("My Name Is Edabit") ➞ "MY NamE IS EdabiT"

capLast("HELp THe LASt LETTERs CAPITALISe") ➞ "HELP THE LAST LETTERS CAPITALISE"
```
### :evergreen_tree: My Code
```js
const capLast = t => t.replace(/[a-z]\b/g, c => c.toUpperCase());
```
