## "EdaBit" Challenge
Create a function that returns the array of numbers from a given range. But for multiples of three, return “Eda” instead of the number and for the multiples of five, return “Bit”. For numbers which are multiples of both three and five, return “EdaBit”.
```js
Examples
edaBit(0, 10) ➞ [0, 1, 2, "Eda", 4, "Bit", "Eda", 7, 8, "Eda", "Bit" ]

edaBit(14, 20) ➞ [14,  "EdaBit", 16, 17,  "Eda", 19, "Bit" ]

edaBit(99, 106) ➞ ["Eda", "Bit", 101, "Eda", 103, 104, "EdaBit", 106 ]
```
Notes
In case the number 0 happens to be in the range, return "EdaBit" as well.
### :barber:My Code
```js
const edaBit = (start, end)=> Array(end - start + 1).fill().map((_, idx) => start + idx)
.map(x=> x === 0 ? "EdaBit" : x %3===0 && x%5===0 ? "EdaBit" : x % 3===0 ? "Eda" 
: x % 5===0 ? "Bit": x);
```

## Convenience Store
Given a total due and an array representing the amount of change in your pocket, determine whether or not you are able to pay for the item. Change will always be represented in the following order: quarters, dimes, nickels, pennies.

To illustrate: changeEnough([25, 20, 5, 0], 4.25) should yield true, since having 25 quarters, 20 dimes, 5 nickels and 0 pennies gives you 6.25 + 2 + .25 + 0 = 8.50.
```js
Examples
changeEnough([2, 100, 0, 0], 14.11) ➞ false

changeEnough([0, 0, 20, 5], 0.75) ➞ true

changeEnough([30, 40, 20, 5], 12.55) ➞ true

changeEnough([10, 0, 0, 50], 3.85) ➞ false

changeEnough([1, 0, 5, 219], 19.99) ➞ false
```
### :slot_machine:My Code
```js
function changeEnough(change, amountDue) {
	let [q,d,n,p] = change;
	return (q*.25) + (d*.10) + (n*.05) + (p*.01) >= amountDue;
}
```

## Number of Arrays in an Array
Return the total number of arrays inside a given array.
```js
Examples
numOfSubbarrays([[1, 2, 3]]) ➞ 1

numOfSubbarrays([[1, 2, 3], [1, 2, 3], [1, 2, 3]]) ➞ 3

numOfSubbarrays([[1, 2, 3], [1, 2, 3], [1, 2, 3], [1, 2, 3]]) ➞ 4

numOfSubbarrays([1, 2, 3]) ➞ 0
```
### :izakaya_lantern: My Code
```js
const numOfSubbarrays = a => a.filter(x=> x.length).length;
```

## Compare by ASCII Codes
Create a function to that compares two words based on the sum of their ASCII codes and returns the word with the smaller ASCII sum.
```js
Examples
asciiSort(["hey", "man"]) ➞ "man"
// ["h", "e", "y"] ➞ sum([104, 101, 121]) ➞ 326
// ["m", "a", "n"] ➞ sum([109, 97, 110]) ➞ 316

asciiSort(["majorly", "then"]) ➞ "then"

asciiSort(["victory", "careless"]) ➞ "victory"
```
### :performing_arts: My Code
```js
function asciiSort(arr) {
	let a1 = arr[0].split('').
	map(num=>num.charCodeAt()).reduce((total,num)=> total + num);
	
	let a2 = arr[1].split('').
	map(num=>num.charCodeAt()).reduce((total,num)=> total + num);
	
	return a1 < a2 ? arr[0] : arr[1];
}
```
## Multi-division
Create a function, that will for a given a, b, c, do the following:

Add a to itself b times.
Check if the result is divisible by c.
```js
Examples
abcmath(42, 5, 10) ➞ false
// 42+42 = 84,84+84 = 168,168+168 = 336,336+336 = 672, 672+672 = 1344
// 1344 is not divisible by 10

abcmath(5, 2, 1) ➞ true

abcmath(1, 2, 3) ➞ false
```
### :watermelon:My Code
```js
function abcmath(a, b, c) {
 while(a < b) {
  a++;
  a+=a;
 }
 return a % c === 0 ? true : false;
}
```


