## White Spaces Between Lower and Uppercase Letters

Write a function that inserts a white space between every instance of a lower character followed immediately by an upper character.
```js
Examples
insertWhitespace("SheWalksToTheBeach") ➞ "She Walks To The Beach"

insertWhitespace("MarvinTalksTooMuch") ➞ "Marvin Talks Too Much"

insertWhitespace("TheGreatestUpsetInHistory") ➞ "The Greatest Upset In History"
```
### :computer: My Code
```js
const insertWhitespace = s => s.replace(/([a-z])([A-Z])/g,'$1 $2');
 
 //alternate
const insertWhitespace = s => s.replace(/\B([A-Z])/g, ' $1')
```
