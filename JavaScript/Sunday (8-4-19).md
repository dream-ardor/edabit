## Find unique positive Numbers from array.
Write a function that will take an array as an argument and will return a new array with unique positive (more than 0) numbers.
```js
Examples
uniqueArr([-5, 1, -7, -5, -2, 3, 3, -5, -1, -1])➞ [1,3] 

uniqueArr([3, -3, -3, 5, 5, -6, -2, -4, -1, 3]) ➞ [3,5]

uniqueArr([10, 6, -12, 13, 5, 5, 13, 6, 5])➞ [10,6,13,5] 
```
### :white_square_button:My Code
```js
const uniqueArr = arr => [...new Set(arr)].filter(x => x > 0);
```

## ASCII Charts (Part 1: Progress Bar)
Given a character and a value between 0 and 100, return a string that represents a simple progress bar.
```
The value represents a percentage.
The bar should begin and end with "|"
Repeat the character to fill the bar, with each character equivalent to 10%
Use spaces to pad the bar to a length of 10 characters.
A single space comes after the bar, then a message with the % completion (e.g. "Progress: 60%")
If the value is 100, the message should be "Completed!".
```
```js
Examples
progressBar("#", 0)   ➞ "|          | Progress: 0%"

progressBar("=", 40)  ➞ "|====      | Progress: 40%"

progressBar("#", 60)  ➞ "|######    | Progress: 60%"

progressBar(">", 100) ➞ "|>>>>>>>>>>| Completed!"
```
## :white_square_button:My Code
```js
function progressBar(bar, progress) {
  return '|' + bar.repeat(progress/10) +
   ' '.repeat(10 - progress/10) + '| ' +
    (progress == 100 ? "Completed!" : "Progress: "+ progress + "%")
}
```

## Is the Word an Isogram?
An isogram is a word that has no repeating letters, consecutive or nonconsecutive. Create a function that takes a string and returns either true or false depending on whether or not it's an "isogram".
```js
Examples
isIsogram("Algorism") ➞ true

isIsogram("PasSword") ➞ false (not case sensitive)

isIsogram("Consecutive") ➞ false
```
### :white_square_button:My Code
```js
const isIsogram = str => str.length == (new Set(str.toLowerCase())).size;

//using regex
const isIsogram = str => !/(\w).*\1/i.test(str);
```

## Remove the Special Characters from a String
Create a function that takes a string, removes all "special" characters (e.g. ! @ # $ % ^ & \ *) and returns the new string. The only non-alphanumeric characters allowed are dashes -, underscores _ and spaces.
```js
Examples
removeSpecialCharacters("The quick brown fox!") ➞ "The quick brown fox"

removeSpecialCharacters("%fd76$fd(-)6GvKlO.") ➞ "fd76fd-6GvKlO"

removeSpecialCharacters("D0n$c sed 0di0 du1") ➞ "D0nc sed 0di0 du1"
```
### :white_square_button:My Code
```js
//regex long way
const removeSpecialCharacters = str => str.replace(/[`~!@#$%^&*()|+\=?;:'",.<>\{\}\[\]\\\/]/g,'');

//regex short way
const removeSpecialCharacters = str => str.replace(/[^\w-_ ]/g,'');
```

