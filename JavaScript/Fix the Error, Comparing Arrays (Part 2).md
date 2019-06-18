## Fix the Error / Comparing Arrays (Part #2)

Create a function that returns true if two arrays contain identical values, and false otherwise.

To solve this question, your friend initially wrote the following code (see this challenge):
```js
function checkEquals(arr1, arr2) {
  if (arr1 === arr2) {
    return true
   } else {
    return false
   }
}
```
If you're unsure why the above code doesn't work, I recommend doing that challenge first.

Your friend did some more research and he fixed the code into the following:
```js
function checkEquals(arr1, arr2) {
  if (arr1.join("") === arr2.join("")) {
    return true
   } else {
    return false
   }
}
```
It works in most cases, but on some cases it fails. This confuses him, can you spot the error and fix it?
```js
Examples
checkEquals([1, 2], [1, 3]) ➞ false

checkEquals([1, 2], [1, 2]) ➞ true

checkEquals([4, 5, 6], [4, 5, 6]) ➞ true

checkEquals([4, 7, 6], [4, 5, 6]) ➞ false

checkEquals([1, 12], [11, 2]) ➞ false
```

## My Code
```js
// Added a space between the quotation marks 
function checkEquals(arr1, arr2) {
	if (arr1.join(" ") === arr2.join(" ")) {
  	return true
 	} else {
  	return false
 	}
}
```
