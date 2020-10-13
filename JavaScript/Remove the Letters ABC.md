## Remove the Letters ABC

Create a function that will remove the letters "a", "b" and "c" from the given string and return the modified version. If the given string does not contain "a", "b", or "c", return null.
```js
Examples
removeABC("This might be a bit hard") ➞ "This might e  it hrd"

removeABC("hello world!") ➞ null

removeABC("") ➞ null
```
### :computer: My Code
```js
const removeABC = s => /[abc]/g.test(s) ? s.replace(/[abc]/g,'') : null
```
