## Count the Capital Letters

Given a string of letters, how many capital letters are there?
```js
Examples
capitalLetters("fvLzpxmgXSDrobbgMVrc") ➞ 6

capitalLetters("JMZWCneOTFLWYwBWxyFw") ➞ 14

capitalLetters("mqeytbbjwqemcdrdsyvq") ➞ 0
```

### :leaves: My Code
```js
const capitalLetters = t =>
  t.split('').filter(x => x == x.toUpperCase()).length;
```
