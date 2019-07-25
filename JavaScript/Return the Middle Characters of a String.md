## Return the Middle Character(s) of a String
Create a function that takes a string and returns the middle character(s). If the word's length is odd, return the middle character. If the word's length is even, return the middle two characters.
```js
Examples
getMiddle("test") ➞ "es"

getMiddle("testing") ➞ "t"

getMiddle("middle") ➞ "dd"

getMiddle("A") ➞ "A"
```

### :dog:My Code
```js
const getMiddle = str => str.length % 2 == 0 ? str.substring((str.length/2), -1,2) 
: str.substring((str.length/2), 1);
```
