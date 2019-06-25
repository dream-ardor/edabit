## Vowel Replacer
Create a function replaces all the vowels in a string with a specified character.
```js
Examples
replaceVowels("the aardvark", "#") ➞ "th# ##rdv#rk"

replaceVowels("minnie mouse", "?") ➞ "m?nn?? m??s?"

replaceVowels("shakespeare", "*") ➞ "sh*k*sp**r*"
```
### My Code :file_folder:
```js
const replaceVowels = (str,ch) => str.replace(/[aeiou]/gi,ch);
```

## Array from Comma-Delimited String
Write a function that turns a comma-delimited list into an array of strings.
```js
Examples
toArray("watermelon, raspberry, orange")
➞ ["watermelon", "raspberry", "orange"]

toArray("x1, x2, x3, x4, x5")
➞ ["x1", "x2", "x3", "x4", "x5"]

toArray("a, b, c, d")
➞ ["a", "b", "c", "d"]

toArray("")
➞ []
```
### My Code :open_file_folder:
```js
const toArray = str => str == ("") ? [] : str.split(", ");
```

## Letters Only
Write a function that removes any non-letters from a string, returning a well-known film title.
```
Examples
lettersOnly("R!=:~0o0./c&}9k`60=y") ➞ "Rocky"

lettersOnly("^,]%4B|@56a![0{2m>b1&4i4") ➞ "Bambi"

lettersOnly("^U)6$22>8p).") ➞ "Up"
```
### My Code :black_nib:	
```js
const lettersOnly = str => str.replace(/[^a-z]/gi,"");
```

## Product of All Odd Integers
Create a function that returns the product of all odd integers in an array.
```js
Examples
oddProduct([3, 4, 1, 1, 5]) ➞ 15

oddProduct([5, 5, 8, 2, 4, 32]) ➞ 25

oddProduct([1, 2, 1, 2, 1, 2, 1, 2]) ➞ 1
```
### My Code :newspaper:
```js
const oddProduct = arr => arr.filter(x => x % 2).reduce((a,b)=> a * b);
```

## Product Divisible By Sum?
Write a function that returns true if the product of an array is divisible by the sum of that same array.
```js
Examples
divisible[3, 2, 4, 2] ➞ false

divisible[4, 2, 6] ➞ true

divisible[3, 5, 1] ➞ false
```
### My Code :video_game:
```js
const divisible = arr => arr.reduce((a,b) => a * b) 
% arr.reduce((a,b)=> a+b) == 0 ? true : false;
```
