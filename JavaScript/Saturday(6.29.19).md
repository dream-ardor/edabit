## Count Instances of a Character in a String
Create a function that takes two strings as arguments and returns the number of times the first string is found in the second string.

Examples
charCount("a", "edabit") ➞ 1

charCount("c", "Chamber of secrets") ➞ 1

charCount("b", "big fat bubble") ➞ 4
### My Code :fire:
```js
const charCount = (myChar, str) => str.split('')
.filter(x => x === myChar).length;
```
## Hashes and Pluses
Create a function that returns the number of hashes and pluses in a string.

Examples
hashPlusCount("###+") ➞ [3, 1]

hashPlusCount("##+++#") ➞ [3, 3]

hashPlusCount("#+++#+#++#") ➞ [4, 6]

hashPlusCount("") ➞ [0, 0]
### My Code :zap:
```js
const hashPlusCount = str => [
(str.match(/#/g) || "").length,
(str.match(/\+/g) || "").length
];
```
## Secret Society
A group of friends have decided to start a secret society. The name will be the first letter of each of their names, sorted in alphabetical order.

Create a function that takes in an array of names and returns the name of the secret society.
```js
Examples
societyName(["Adam", "Sarah", "Malcolm"]) ➞ "AMS"

societyName(["Harry", "Newt", "Luna", "Cho"]) ➞ "CHLN"

societyName(["Phoebe", "Chandler", "Rachel", "Ross", "Monica", "Joey"]) ➞ "CJMPRR"
```

### My Code :cyclone:
```js
const societyName = friends => 
friends.map((x) => x[0]).sort().join('').toUpperCase();

```

