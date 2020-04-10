## Changing a String into camelCase

Using Camel Case (or camelCase) is where the first word is in lower case, and all words after it have their first letter capitalised. Note that there are no spaces in between words!

Create a function that takes a string and returns it back in camelCase.
```js
Examples
camelCasing("Hello World") ➞ "helloWorld"

camelCasing("snake_case") ➞ "snakeCase"

camelCasing("low high_HIGH") ➞ "lowHighHigh"

Notes:
You need to remove all spaces and underscores.
There will be no numbers in inputs.
```
### :computer: My Code
```js
const camelCasing = s =>
 s.toLowerCase().replace(/[^a-zA-Z0-9]+(.)/g, (a,b) => b.toUpperCase());
```
