## Bitwise Operations
A decimal number can be represented as a sequence of bits. To illustrate:
```js
6  = 00000110
23 = 00010111
```
From the bitwise representation of numbers, we can calculate the bitwise AND, bitwise OR and bitwise XOR. Using the example above:
```js
bitwiseAND(6, 23)➞ 00000110
bitwiseOR(6, 23) ➞ 00010111
bitwiseXOR(6, 23) ➞ 00010001
```
Write 3 functions to calculate the bitwise AND, bitwise OR and bitwise XOR of two numbers.
```
Examples
bitwiseAND(7, 12) ➞ 4

bitwiseOR(7, 12) ➞ 15

bitwiseXOR(7, 12) ➞ 11
```
### :yen:My Code
```js
const bitwiseAND = (n1, n2) => n1&n2;
const bitwiseOR = (n1, n2) => n1|n2;
const bitwiseXOR = (n1, n2) => n1^n2;
```
## Count Instances of a Character in a String
Create a function that takes two strings as arguments and returns the number of times the first string is found in the second string.
```js
Examples
charCount("a", "edabit") ➞ 1

charCount("c", "Chamber of secrets") ➞ 1

charCount("b", "big fat bubble") ➞ 4
```
### :sake:My Code
```js
let charCount = (myChar, str) =>
str.split('').filter(x => x == myChar).length;
```

## Regex Series: 5-Digit Zip Code
Write a regular expression that matches a string if and only if it is a valid zip code.
```js
Examples
"32554" ➞ true

"92 342" ➞ false
// Invalid: contains a whitespace

"9@342" ➞ false
// Invalid: contains a non-numeric character

"923444" ➞ false
// Invalid: length is not 5
```
Notes
Zipcodes must be 5 digits long exactly and only contain numbers.
Not allowed: non-numeric characters or whitespaces.
This challenge is designed to use Regex only.
### :beers:My Code
```js
let x = /^\d{5}$/;
```

## Spelling it Out
Create a function which takes in a word and spells it out, by consecutively adding letters until the full word is completed.
```js
Examples
spelling("bee") ➞ ["b", "be", "bee"]

spelling("happy") ➞ ["h", "ha", "hap", "happ", "happy"]

spelling("eagerly") ➞ ["e", "ea", "eag", "eage", "eager", "eagerl", "eagerly"]
```
### :tropical_drink:My Code
```js
const spelling = str =>
str.split('').map((a,b)=> str.slice(0, b + 1));
```
## Join Two Portions of a Path
Write a function that receives two portions of a path and joins them. The portions will be joined with the "/" separator. There could be only one separator and if it is not present it should be added.
```js
Examples
joinPath("portion1", "portion2") ➞ "portion1/portion2"

joinPath("portion1/", "portion2") ➞ "portion1/portion2"

joinPath("portion1", "/portion2") ➞ "portion1/portion2"

joinPath("portion1/", "/portion2") ➞ "portion1/portion2"
```
### :cocktail:My Code
```js
const joinPath = (portion1, portion2) =>
portion1.replace("/", "") + "/" + portion2.replace("/", "");
```

## Repeating Letters
Create a function that takes a string and returns a string in which each character is repeated once.
```js
Examples
doubleChar("String") ➞ "SSttrriinngg"

doubleChar("Hello World!") ➞ "HHeelllloo  WWoorrlldd!!"

doubleChar("1234!_ ") ➞ "11223344!!__  "
```
### :wine_glass:My Code
```js
const doubleChar = str => str.split('').map(x => x + x).join('');
```

## Valid Zip Code
Zip codes consist of 5 consecutive digits. Given a string, write a function to determine whether the input is a valid zip code.
```js
Examples
isValid("59001") ➞ true

isValid("853a7") ➞ false

isValid("732 32") ➞ false

isValid("393939") ➞ false
```
### :fork_and_knife:My Code
```js
const isValid = zip => /^\d{5}$/.test(zip);
```

