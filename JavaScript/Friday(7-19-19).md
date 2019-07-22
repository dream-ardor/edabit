## Longest Sequence of Consecutive Zeroes
Write a function that returns the longest sequence of consecutive zeroes in a binary string.
```js
Examples
longestZero("01100001011000") ➞ "0000"

longestZero("100100100") ➞ "00"

longestZero("11111") ➞ ""
```
### :arrow_forward:My Code
```js
const longestZero = s =>  s.split('1').reduce((a, b) => a.length > b.length ? a : b);
```

## Get the Century
Create a function that takes in a date and returns the correct century.
```js
Examples
century(1756) ➞ "18th century"

century(1555) ➞ "16th century"

century(1000) ➞ "10th century"

century(1001) ➞ "11th century"

century(2005) ➞ "21st century"
```
### :arrow_down:My Code
```js
const century = year =>  year < 2001 ? Math.ceil(year/100)  + "th century"
:Math.ceil(year/100) + "st century";
```

## Mean of All Digits
Create a function that returns the mean of all digits.
```js
Examples
mean(42) ➞ 3

mean(12345) ➞ 3

mean(666) ➞ 6
```
### :1234:My Code
```js
const mean = num => {
let n1 = Math.abs(num).toString().split('').map(a=>Number(a));
return n1.reduce((a,b)=>a+b)/n1.length;
}
```

## Apples and Bananas
Write a function, .vreplace() that extends the String prototype by replacing all vowels in a string with a specified vowel.
```js
Examples
"apples and bananas".vreplace("u") ➞ "upplus und bununus"

"cheese casserole".vreplace("o") ➞ "chooso cossorolo"

"stuffed jalapeno poppers".vreplace("e") ➞ "steffed jelepene peppers"
```
### :capital_abcd:My Code
```js
String.prototype.vreplace = function(vowel) {
	return this.replace(/[aeiou]/g, vowel);
}
```

## Find the Minimum, Maximum, Length and Average Values
Create a function that takes an array of numbers and returns the following statistics:
```
Minimum Value
Maximum Value
Sequence Length
Average Value
```
```js
Examples
minMaxLengthAverage([6, 9, 15, -2, 92, 11]) ➞ [-2, 92, 6, 21.833333333333332]

minMaxLengthAverage([30, 43, 20, 92, 3, 74]) ➞ [3, 92, 6, 43.666666666666664]

minMaxLengthAverage([4.54, 8.32, 5.20]) ➞ [4.54, 8.32, 3, 6.02]
```
### :arrows_clockwise:My Code
```js
function minMaxLengthAverage(arr) {
	let a = Math.min(...arr);
	let b = Math.max(...arr);
	let c = arr.length;
	let d = arr.reduce((a1,b1)=>a1+b1)/arr.length;
	return [a,b,c,d];
}
```

## Reverse Words Starting With a Particular Letter
Write a function that reverses all the words in a sentence starting with a particular letter.
```js
Examples
specialReverse("word searches are super fun", "s")
➞ "word sehcraes are repus fun"

specialReverse("first man to walk on the moon", "m")
➞ "first nam to walk on the noom"

specialReverse("peter piper picked pickled peppers", "p")
➞ "retep repip dekcip delkcip sreppep"
```

### :u7a7a:My Code
```js
const specialReverse = (s, c) => s.split(' ').map(a=> a[0] == c
? a.split('').reverse().join(''):a).join(' ');
```

## Even or Odd Number of Factors
Create a function that returns "even" if a number has an even number of factors and "odd" if a number has an odd number of factors.
```js
Examples
factorGroup(33) ➞ "even"

factorGroup(36) ➞ "odd"

factorGroup(7) ➞ "even"
```
### :u7533:My Code
```js
const factorGroup = num => Math.sqrt(num) % 1 ? "even" : "odd";
```
