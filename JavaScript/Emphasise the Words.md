## Emphasise the Words

Create a function that returns a capitalized version of the string passed. The first letter of each word in the string should be capitalized while the rest of each word should be lowercase.
```js
Examples
emphasise("hello world") ➞ "Hello World"

emphasise("GOOD MORNING") ➞ "Good Morning"

emphasise("99 red balloons!") ➞ "99 Red Balloons!"
```
### :palm_tree: My Code
```js
const emphasise = s => s.toLowerCase().replace(/\b\w/g, a => a.toUpperCase());


//alternate solutions
const emphasise = s => s.toLowerCase().replace(/(^\w{1})|(\s{1}\w{1})/g, a => a.toUpperCase());
 
const emphasise = (str) => str ? str.split(' ').map(s => s.charAt(0).toUpperCase() + s.substring(1).toLowerCase()).join(' ') : "";
 
```
