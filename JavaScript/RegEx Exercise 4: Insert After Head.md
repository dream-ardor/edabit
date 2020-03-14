## RegEx Exercise 4: Insert after head
```js
Challenge:
Write a regular expression that inserts <h1>Hello</h1> immediately after <body> tag.
The tag may have attributes.
You only have to come up with the regular expression. The replace function is already done (see the Tests tab)
const REGEXP = /your regular expression/

let str = "<html><body style="height: 200px"> ... </body></html>"

str = str.replace(REGEXP, `<h1>Hello</h1>`);

console.log(str) ➞ <html> <body style="height: 200px"><h1>Hello</h1> ... </body> </html>
```
### :leaves: My Code
```js
const REGEXP = /(?<=<body.*>)/
```
