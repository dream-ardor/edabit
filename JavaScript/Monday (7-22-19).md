## Double Letters
Create a function that takes a word and returns true if the word has two consecutive identical letters.
```js
Examples
doubleLetters("loop") ➞ true

doubleLetters("yummy") ➞ true

doubleLetters("orange") ➞ false

doubleLetters("munchkin") ➞ false
```
### :wrench:My Code
```js
const doubleLetters = w => /(.)\1+/.test(w);
```

## Is Johnny Making Progress?
To train for an upcoming marathon, Johnny goes on one long-distance run each Saturday. He wants to track how often the number of miles he runs this Saturday exceeds the number of miles run the previous Saturday. This is called a progress day.

Create a function that takes in an array of miles run every Saturday and returns Johnny's total number of progress days.
```js
Examples
progressDays([3, 4, 1, 2]) ➞ 2
// There are two progress days, (3->4) and (1->2)

progressDays([10, 11, 12, 9, 10]) ➞ 3

progressDays([6, 5, 4, 3, 2, 9]) ➞ 1

progressDays([9, 9])  ➞ 0
```
### :nut_and_bolt:My Code
```js
const progressDays = runs => runs.filter((run,i,arr)=>
run < arr[i+1]).length;

//using for loop
const progressDays = runs => {
 let a = 0;
  for(i=0; i < runs.length; i++) {
   if (runs[i+1] > runs[i]) a++
  }
   return a;
}
```

## Capitalize the Names
Create a function that takes an array of names and returns an array with the first letter capitalized.
```js
Examples
capMe(["mavis", "senaida", "letty"]) ➞ ["Mavis", "Senaida", "Letty"]

capMe(["samuel", "MABELLE", "letitia", "meridith"]) ➞ ["Samuel", "Mabelle", "Letitia", "Meridith"]

capMe(["Slyvia", "Kristal", "Sharilyn", "Calista"]) ➞ ["Slyvia", "Kristal", "Sharilyn", "Calista"]
```
### :hammer:My Code
```js
const capMe = arr => arr.map(x => x.charAt(0).toUpperCase() + x.substring(1).toLowerCase());
```

## Remove Duplicates from an Array
Create a function that takes an array of items, removes all duplicate items and returns a new array in the same sequential order as the old array (minus duplicates).
```js
Examples
removeDups(["John", "Taylor", "John"]) ➞ ["John", "Taylor"]

removeDups([1, 0, 1, 0]) ➞ [1, 0]

removeDups(["The", "big", "cat"]) ➞ ["The", "big", "cat"]
```
### :electric_plug:My Code
```js
const removeDups = arr => [...new Set(arr)];
```


