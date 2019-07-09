## Find the Index (Part 2)
Create a function that finds the index of a given item if the array is sorted.
```js
Examples
search([1, 2, 3, 4], 3) ➞ 2

search([2, 4, 6, 8, 10], 8) ➞ 3

search([1, 3, 5, 7, 9], 11) ➞ -1
```
### :shoe:My Code
```js
const search = (arr, item) => arr.includes(item) ?
arr.indexOf(item) : -1;
```

## Add, Subtract, Multiply or Divide?
Write a function that takes two numbers and returns if they should be added, subtracted, multplied or divided to get 24. If none of the operations can give 24, return null.
```js
Examples
operation(15, 9) ➞ "added"

operation(26, 2) ➞ "subtracted"

operation(11, 11) ➞ null
```
### :boot:My Code
```js
const operation = (n1, n2) =>
n1 + n2 == 24 ? "added" : n1 - n2 == 24 ? "subtracted":
n1 * n2 == 24 ? "multiplied" : n1 / n2 == 24 ? "divided" : null;
```

## Extract City Facts
Create a function that takes an object as an argument and returns a string with facts about the city. The city facts will need to be extracted from the object's three properties:
```
name
population
continent
```
The string should have the following format: X has a population of Y and is situated in Z (where X is the city name, Y is the population and Z is the continent the city is situated in).
```js
Examples
cityFacts({
  name: "Paris",
  population: "2,140,526",
  continent: "Europe"
}) ➞ "Paris has a population of 2,140,526 and is situated in Europe"

cityFacts({
  name: "Tokyo",
  population: "13,929,286",
  continent: "Asia"
}) ➞ "Tokyo has a population of 13,929,286 and is situated in Asia"
```
### :saxophone:My Code
```js
const cityFacts = city => city.name + " has a population of " 
+ city.population + " and is situated in " + city.continent;
```

## Recursion: Sum
Write a function that recursively finds the sum of the first n natural numbers.
```js
Examples
sum(5) ➞ 15
// 1 + 2 + 3 + 4 + 5 = 15

sum(1) ➞ 1

sum(12) ➞ 78
```
### :dart:My Code
```js
const sum = n => n <= 1 ? n : n + sum(n-1);
```

## Hamming Distance
Hamming distance is the number of characters that differ between two strings.

To illustrate:
```js
String1: "abcbba"
String2: "abcbda"
```
Hamming Distance: 1 - "b" vs. "d" is the only difference.
Create a function that computes the hamming distance between two strings.
```js
Examples
hammingDistance("abcde", "bcdef") ➞ 5

hammingDistance("abcde", "abcde") ➞ 0

hammingDistance("strong", "strung") ➞ 1
```
### :guitar:My Code
```js
function hammingDistance(s1, s2) {
	let dis = 0;
	for(i = 0; i < s1.length; i += 1) {
		if (s1[i]!== s2[i] ) {
			dis += 1;
		}
	}
	return dis;
}
```

## Recursion: Array Sum
Write a function that recursively finds the sum of an array.
```js
Examples
sum([1, 2, 3, 4]) ➞ 10

sum([1, 2]) ➞ 3

sum([1]) ➞ 1

sum([]) ➞ 0
```
### :lipstick:My Code
```js
const sum = arr => arr.length === 0 ? 0 : arr[0] + sum(arr.slice(1));
```

## Recursion: Reverse a String
Write a function that reverses a string recursively.
```js
Examples
reverse("hello") ➞ "olleh"

reverse("world") ➞ "dlrow"

reverse("a") ➞ "a"

reverse("") ➞ ""
```
Notes
For non-base cases, your function must call itself at least once.
### :high_heel:My Code
```js
const reverse = str => str === "" ? str : str.split('').reverse().join('');
```

## Don't Get Too Distracted!
I'm trying to watch some lectures to study for my next exam but I keep getting distracted by meme compilations, vine compilations, anime, and more on my favorite video platform.

Your job is to help me by creating a function that takes in a String and checks to see if it contains the following words or phrases:
```
"anime"
"meme"
"vine"
"roasts"
"Danny Devito"
```
If is does, return "NO!". Otherwise, return "Safe watching!".
```js
Examples
preventDistractions("vines that butter my eggroll") ➞ "NO!"

preventDistractions("Hot pictures of Danny Devito") ➞ "NO!"

preventDistractions("How to ace BC Calculus in 5 Easy Steps") ➞ "Safe watching!"
```

### :sandal:My Code
```js
const preventDistractions = str =>
str.includes("anime") || str.includes("meme") ||
str.includes("vine") || str.includes("roasts") ||
str.includes("Danny Devito") ? "NO!" : "Safe watching!";

//solution using regex
```js
const preventDistractions = str =>
/anime|vine|roasts|meme|Danny Devito/.test(str) ? 
"NO!" : "Safe watching!";
```
