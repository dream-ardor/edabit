## Reverse the Order of Words with Five Letters or More
Write a function that takes a string of one or more words as an argument and returns the same string, but with all five or more letter words reversed. Strings passed in will consist of only letters and spaces. Spaces will be included only when more than one word is present.
```js
Examples
reverse("Reverse") ➞ "esreveR"

reverse("This is a typical sentence.") ➞ "This is a lacipyt .ecnetnes"

reverse("The dog is big.") ➞ "The dog is big."
```
### :stars:My Code
```js
const reverse = str => str.split(' ')
.map(x => x.length >= 5 ? x.split('').reverse().join('') : x).join(' ');
```

## Snail Race
Steve and Maurice are racing snails. They each have 3, a slow (s), medium (m) and fast (f) one. Although Steve's snails are all a bit stronger than Maurice's, Maurice has a trick up his sleeve. His plan is (written [Maurice, Steve]):
```
Round 1: [s, f] Sacrifice his slowest snail against Steve's fastest.
Round 2: [m, s] Use his middle snail against Steve's slowest.
Round 3: [f, m] Use his fastest snail against Steve's middle.
```
Create a function that determines whether Maurice's plan will work by outputting true if Maurice wins 2/3 games.

The function inputs:
```js
Array 1: [s, m, f] for Maurice.
Array 2: [s, m, f] for Steve.
```
```js
Examples
mauriceWins([3, 5, 10], [4, 7, 11]) ➞ true
// Since the matches are (3, 11), (5, 4) and (10, 7), Maurice wins 2 out of 3.

mauriceWins([6, 8, 9], [7, 12, 14]) ➞ false
// Since the matches are (6, 14), (8, 7) and (9, 12), Steve wins 2 out of 3.

mauriceWins([1, 8, 20], [2, 9, 100]) ➞ true
```
### :stars:My Code
```js
const mauriceWins = (ms, ss) => (ms[1] > ss [0] && ms[2] > ss[1]);
```

## Maskify the String
Usually when you sign up for an account to buy something, your credit card number, phone number or answer to a secret question is partially obscured in some way. Since someone could look over your shoulder, you don't want that shown on your screen. Hence, the website masks these strings.

Your task is to create a function that takes a string, transforms all but the last four characters into "#" and returns the new masked string.
```js
Examples
maskify("4556364607935616") ➞ "############5616"

maskify("64607935616") ➞ "#######5616"

maskify("1") ➞ "1"

maskify("") ➞ ""
```
### :stars:My Code
```js
function maskify(str) {
  let a = str.slice(0,-4).replace(/(.)/g, "#")
  let b = str.slice(-4);
   return a+b;
}
```

## Sum of all Evens in a Matrix
Create a function that returns the sum of all even elements in a 2D matrix.
```js
Examples
sumOfEvens([
  [1, 0, 2],
  [5, 5, 7],
  [9, 4, 3]
]) ➞ 6

// 2 + 4 = 6

sumOfEvens([
  [1, 1],
  [1, 1]
]) ➞ 0

sumOfEvens([
  [42, 9],
  [16, 8]
]) ➞ 66

sumOfEvens([
  [],
  [],
  []
]) ➞ 0
```
### :stars:My Code
```js
const sumOfEvens = arr => [].concat(...arr)
.filter(x => x % 2 === 0)
.reduce((a,b) => a + b, 0);   

```

## Check for Anagrams
Create a function that takes two strings and returns (true or false) whether they're anagrams or not.
```js
Examples
isAnagram("cristian", "Cristina") ➞ true

isAnagram("Dave Barry", "Ray Adverb") ➞ true

isAnagram("Nope", "Note") ➞ false
```
### :stars:My Code
```js
const isAnagram = (s1, s2) =>
s1.toLowerCase().split('').sort().join('') ==
s2.toLowerCase().split('').sort().join('')
```
