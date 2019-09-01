## Return the Index of All Capital Letters
Create a function that takes a single string as argument and returns an ordered array containing the indexes of all capital letters in the string.
```js
Examples
indexOfCaps("eDaBiT") ➞ [1, 3, 5]

indexOfCaps("eQuINoX") ➞ [1, 3, 4, 6]

indexOfCaps("determine") ➞ []

indexOfCaps("STRIKE") ➞ [0, 1, 2, 3, 4, 5]

indexOfCaps("sUn") ➞ [1]
```
### :dark_sunglasses: My Code
```js
const indexOfCaps = s => {
  let a = [];
   for(i = 0; i < s.length; i++) {
    if (s[i].match(/[A-Z]/g)) {
     a.push(i)
  }
}
  return a;
}
```

## Check if One Array can be Nested in Another
Create a function that returns true if the first array can be nested inside the second.

arr1 can be nested inside arr2 if:

arr1's min is greater than arr2's min.
arr1's max is less than arr2's max.
```js
Examples
canNest([1, 2, 3, 4], [0, 6]) ➞ true

canNest([3, 1], [4, 0]) ➞ true

canNest([9, 9, 8], [8, 9]) ➞ false

canNest([1, 2, 3, 4], [2, 3]) ➞ false
```
### :dark_sunglasses: My Code
```js
const canNest = (a1, a2) =>
 Math.min(...a1) > Math.min(...a2) && Math.max(...a1) < Math.max(...a2);
```

## Remove Surrounding Duplicate Items
Create a function that takes a sequence of either strings or numbers, removes the surrounding duplicates and returns an array of items without any items with the same value next to each other and preserves the original order of items.
```js
Examples
uniqueInOrder("AAAABBBCCDAABBB") ➞ ["A", "B", "C", "D", "A", "B"]

uniqueInOrder("ABBCcAD") ➞ ["A", "B", "C", "c", "A", "D"]

uniqueInOrder([1, 2, 2, 3, 3]) ➞ [1, 2, 3]
```
### :dark_sunglasses: My Code
```js
const uniqueInOrder = s => [...s].filter((a,b)=> a != s[b+1]);

//longer way
const uniqueInOrder = s => {
 let a = [];
  a.push(s[0]);
   for(var i = 0; i < s.length -1; i++) {
    if(s[i] != s[i + 1]) {
      a.push(s[i + 1]);
     }
  }
  return a;
}
```

## Stand in Line
Write a function that takes an array and a number as arguments. Add the number to the end of the array, then remove the first element of the array. The function should then return the updated array.
```js
Examples
nextInLine([5, 6, 7, 8, 9], 1) ➞ [6, 7, 8, 9 ,1]

nextInLine([7, 6, 3, 23, 17], 10) ➞ [6, 3, 23, 17, 10]

nextInLine([1, 10, 20, 42 ], 6) ➞ [10, 20, 42, 6]

nextInLine([], 6) ➞ "No array has been selected"
```

### :dark_sunglasses: My Code
```js
function nextInLine(a, n) {
 if(!a) {return "No array has been selected"}
  a.push(n);
  a.shift();
   return a;
}
//shorter version using ES6
const nextInLine = (a, n) => 
a ? a.slice(1).concat(n) : `No array has been selected`;
```

## Days in a Month
Create a function that takes the month and year (as integers) and returns the number of days in that month.
```js
Examples
days(2, 2018) ➞ 28

days(4, 654) ➞ 30

days(2, 200) ➞ 28

days(2, 1000) ➞ 29
```
### :dark_sunglasses: My Code
```js
const days = (month, year) => new Date(year, month, 0).getDate();
```

## Flash Cards
Create a function that outputs the results of a flashcard. A flashcard is an array of three elements: a number, an operator symbol, and another number. Return the mathematical result of that expression.

There are 4 operators: + (addition), - (subtraction), x (multiplication), and / (division). If the flashcard displays a number being divided by zero, e.g. [3, "/", 0], then return undefined. For division, round to the hundredths place. So [10, "/", 3] should return 3.33.
```js
Examples
flash([3, "x", 7]) ➞ 21

flash([5, "+", 7]) ➞ 12

flash([10, "-", 9]) ➞ 1

flash([10, "/", 0]) ➞ undefined

flash([10, "/", 3]) ➞ 3.33
```
### :dark_sunglasses: My Code
```js
const flash = ([n1, op, n2]) => 
op === '/' && n2 == 0 ? undefined :
op === 'x' ? n1 * n2 :
op === '-' ? n1 - n2 :
op === '+' ? n1 + n2 :
+(n1 / n2).toFixed(2);
```


