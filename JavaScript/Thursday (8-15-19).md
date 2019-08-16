## Both zero, negative or positive
Write a function that checks if two numbers are either both smaller than 0, both 0 or both greater than 0.
```js
Examples
both(6, 2) ➞ true

both(0, 0) ➞ true

both(-1, 2) ➞ false
```
### :stars: My Code
```js
const both = (n1, n2) => n1 == 0 && n2 == 0 || n1 > 0 && n2 > 0 || n1 < 0 && n2 < 0;
```

## Return the Objects Keys and Values
Create a function that takes an object and returns the keys and values as separate arrays.
```js
Examples
keysAndValues({ a: 1, b: 2, c: 3 })
➞ [["a", "b", "c"], [1, 2, 3]]

keysAndValues({ a: "Apple", b: "Microsoft", c: "Google" })
➞ [["a", "b", "c"], ["Apple", "Microsoft", "Google"]]

keysAndValues({ key1: true, key2: false, key3: undefined })
➞ [["key1", "key2", "key3"], [true, false, undefined]]
```
### :stars: My Code
```js
//long way
function keysAndValues(obj) {
	let a = [],
     b = [];
for (property in obj) {
   if ( ! obj.hasOwnProperty(property)) {
    continue;
   }
   a.push(property);
   b.push(obj[property]);
}
	return [a, b];
}

// short way
const keysAndValues = obj => 
[Object.keys(obj), Object.keys(obj).map(x => obj[x])];
```

## Get the Date
Write a function that, given a date (in the format MM/DD/YYYY), returns the day of the week as a string. Each day name must be one of the following strings: "Sunday", "Monday", "Tuesday", "Wednesday", "Thursday", "Friday", or "Saturday".

To illustrate, the day of the week for "12/07/2016" is "Wednesday".
```js
Examples
getDay("12/07/2016") ➞ "Wednesday"

getDay("09/04/2016)" ➞ "Sunday"

getDay("12/08/11") ➞ "Thursday"
```
### :stars: My Code
```js
const getDay = d => new Date(d).toLocaleString('en', {weekday:'long'});
```
## Split Item Codes
You have an array of item codes with the following format: "[letters][digits]"

Create a function that splits these strings into their alphabetic and numeric parts.
```js
Examples
splitCode("TEWA8392") ➞ ["TEWA", 8392]

splitCode("MMU778") ➞ ["MMU", 778]

splitCode("SRPE5532") ➞ ["SSRPE", 5532]
```
### :stars: My Code
```js
const splitCode = i =>
[i.match(/[A-Z]/g).join(''), +i.match(/\d/g).join('')];
```
## Check if a Number is Prime
Create a function that outputs true if a number is prime, and false otherwise.
```js
Examples
isPrime(31) ➞ true

isPrime(18) ➞ false

isPrime(11) ➞ true
```
### :stars: My Code
```js
function isPrime(n) {
  if(n == 1) return false;
   for(i = 2; i < n; i++) {if(n % i === 0) return false};
  return true;
}
```


