## City School Creating IDS

Many IDS (for emails or Google ID) are created using the person's name.

Create a function that will return a four-character ID using the person's first name and last name. The first character will be the first letter of the first name but in lowercase. The next three characters will be the first three characters of the last name, but the first letter will be capitalized and the other two will be in lower case.
```js
Examples
createID("mary", "lamb") ➞ "mLam"

createID("John", "SMITH") ➞ "jSmi"

createID("mary", "smith") ➞ "mSmi"
```
### :leaves: My Code
```js
const createID = (f,l) => f[0].toLowerCase() + l[0].toUpperCase() + l.slice(1,3).toLowerCase();
```
