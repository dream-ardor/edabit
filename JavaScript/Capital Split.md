## Capital Split

Create a function which adds spaces before every capital in a word. Uncapitalize the whole string afterwards.
```js
Examples
capSpace("helloWorld") ➞ "hello world"

capSpace("iLoveMyTeapot") ➞ "i love my teapot"

capSpace("stayIndoors") ➞ "stay indoors"
```
### :sunny: My Code
```js
const capSpace = t => t.replace(/([A-Z])/g, ' $1').toLowerCase();
```
