## Is the Average of All Elements a Whole Number?
Create a function that takes an array as an argument and returns true or false depending on whether the average of all elements in the array is a whole number or not.
```js
Examples
isAvgWhole([1, 3]) ➞ true

isAvgWhole([1, 2, 3, 4]) ➞ false

isAvgWhole([1, 5, 6]) ➞ true

isAvgWhole([1, 1, 1]) ➞ true

isAvgWhole([9, 2, 2, 5]) ➞ false
```
### :rice_ball:My Code
```js
const isAvgWhole = arr => Number.isInteger(arr.reduce((a,b)=> a+b) / arr.length);
```

## Find the Largest Numbers in a Group of Arrays
Create a function that takes an array of arrays with numbers. Return a new (single) array with the largest numbers of each.
```
Examples
findLargestNums([[4, 2, 7, 1], [20, 70, 40, 90], [1, 2, 0]]) ➞ [7, 90, 2]

findLargestNums([[-34, -54, -74], [-32, -2, -65], [-54, 7, -43]]) ➞ [-34, -2, 7]

findLargestNums([[0.4321, 0.7634, 0.652], [1.324, 9.32, 2.5423, 6.4314], [9, 3, 6, 3]]) ➞ [0.7634, 9.32, 9]
```
### :rice:My Code
```js
const findLargestNums = arr => arr.map(x => Math.max(...x));
```

## Remove Duplicates from an Array
Create a function that takes an array of items, removes all duplicate items and returns a new array in the same sequential order as the old array (minus duplicates).
```js
Examples
removeDups(["John", "Taylor", "John"]) ➞ ["John", "Taylor"]

removeDups([1, 0, 1, 0]) ➞ [1, 0]

removeDups(["The", "big", "cat"]) ➞ ["The", "big", "cat"]
```
### :ramen:My Code
```js
let removeDups = arr => [...new Set(arr)];
```

## Capitalize by ASCII
Create a function that takes a string as input and capitalizes a letter if it's ASCII code is even, and returns its lower case version if it's ASCII code is odd.
```js
Examples
asciiCapitalize("to be or not to be!") ➞ "To Be oR NoT To Be!"

asciiCapitalize("THE LITTLE MERMAID") ➞ "THe LiTTLe meRmaiD"

asciiCapitalize("Oh what a beautiful morning.") ➞ "oH wHaT a BeauTiFuL moRNiNg."
```
### :curry:My Code
```js
const asciiCapitalize = str =>
str.split('').map(x => x.charCodeAt() % 2 === 0 ? x.toUpperCase() : x.toLowerCase()).join('');
```

## Something in the Box?
Create a function that returns true if an asterisk * is inside a box.
```
Examples
inBox([
  "###",
  "#*#",
  "###"
]) ➞ true

inBox([
  "####",
  "#* #",
  "#  #",
  "####"
]) ➞ true

inBox([
  "####",
  "#  #",
  "#  #",
  "####"
]) ➞ false

inBox([
  "#####",
  "#   #",
  "#   #",
  "#   #",
  "#####"
]) ➞ false
```
### :egg:My Code
```js
function inBox(arr) {
	for(i=0; i<arr.length; i++) {
		if (arr[i].includes('*')) {
			return true;
		}
	}
	return false;
}
//using join and includes
let inBox = arr =>  arr.join("").includes("*");

//using regex
const inBox = a => a.some(e => (/\*/).test(e));
```


