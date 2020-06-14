Middle Character Of a String
Create a function that returns the middle character of the string.
```js
Examples
middleCharacter('balkot') ➞ 'l'

middleCharacter('himani') ➞ 'm'

middleCharacter('nepali') ➞ 'p'

middleCharacter('java') ➞ 'a'

middleCharacter('kane') ➞ 'a'

middleCharacter('stoned') ➞ 'o'
```
### :computer: My Code
```js
const middleCharacter = t => t.substr(t.length - 1 >>> 1, (~t.length & 1));

//alternate
const middleCharacter = s => s[(s.length >> 1) - 1];
```
