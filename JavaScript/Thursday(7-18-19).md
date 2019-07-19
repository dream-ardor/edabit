## Special Arrays
An array is special, if every even index contains an even number and every odd index contains an odd number. Create a function that returns true if an array is special, and false otherwise.
```js
Examples
isSpecialArray([2, 7, 4, 9, 6, 1, 6, 3]) ➞ true
// Even indices: [2, 4, 6, 6]; Odd indices: [7, 9, 1, 3]

isSpecialArray([2, 7, 9, 1, 6, 1, 6, 3]) ➞ false
// Index 2 has an odd number 9.

isSpecialArray([2, 7, 8, 8, 6, 1, 6, 3]) ➞ false
// Index 3 has an even number 8.
```
### :hamburger:My Code
```js
const isSpecialArray = arr => arr.every((a,b)=>
a % 2 ==0 && b % 2==0 ? true:
a % 2 !== 0 && b % 2 !== 0 ? true : false);
```

## Transform Upvotes
Create a function that transforms a string of upvote counts into an array of numbers. Each k represents a thousand.
```js
Examples
transformUpvotes("6.8k 13.5k") ➞ [6800, 13500]

transformUpvotes("5.5k 8.9k 32") ➞ [5500, 8900, 32]

transformUpvotes("20.3k 3.8k 7.7k 992") ➞ [20300, 3800, 7700, 992]
```
### :fries:My Code
```js
const transformUpvotes = str => str.split(" ").map(num =>
num.includes('k') ? parseFloat(num, 10) * 1000 : num * 1);
```

## Odd Up, Even Down — N Times
Create a function that performs an even-odd transform to an array, n times. Each even-odd transformation:

Adds two (+2) to each odd integer.
Subtracts two (-2) to each even integer.
```js
Examples
evenOddTransform([3, 4, 9], 3) ➞ [9, -2, 15]
// Since [3, 4, 9] ➞ [5, 2, 11] ➞ [7, 0, 13] ➞ [9, -2, 15]

evenOddTransform([0, 0, 0], 10) ➞ [-20, -20, -20]

evenOddTransform([1, 2, 3], 1) ➞ [3, 0, 5]
```
### :oden:My Code
```js
const evenOddTransform = (arr, n) =>
arr.map(x => x % 2 ? x + (2*n) : x - (2*n));
```

## Factor Chain
A factor chain is an array where each previous element is a factor of the next consecutive element. The following is a factor chain:
```
[3, 6, 12, 36]

// 3 is a factor of 6
// 6 is a factor of 12
// 12 is a factor of 36
```
Create a function that determines whether or not an array is a factor chain.
```js
Examples
factorChain([1, 2, 4, 8, 16, 32]) ➞ true

factorChain([1, 1, 1, 1, 1, 1]) ➞ true

factorChain([2, 4, 6, 7, 12]) ➞ false

factorChain([10, 1]) ➞ false
```
### :egg:My Code
```js
const factorChain=arr=>arr.reduce((a,v,i)=> v % arr[i-1] == 0);
```

## Phone Number Formatting
Create a function that takes an array of 10 numbers (between 0 and 9) and returns a string of those numbers formatted as a phone number (e.g. (555) 555-5555).
```js
Examples
formatPhoneNumber([1, 2, 3, 4, 5, 6, 7, 8, 9, 0]) ➞ "(123) 456-7890"

formatPhoneNumber([5, 1, 9, 5, 5, 5, 4, 4, 6, 8]) ➞ "(519) 555-4468"

formatPhoneNumber([3, 4, 5, 5, 0, 1, 2, 5, 2, 7]) ➞ "(345) 501-2527"
```

### :pizza:My Code
```js
const formatPhoneNumber = numbers => numbers.join('').replace(/(\d{3})(\d{3})/, '($1) $2-');
```
## Detect Browser from User Agent
You need to detect what browser is being used. Create a function that takes a string (browser identifier) and returns the browser name.
```js
Examples
detectBrowser("Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/67.0.3396.87 Safari/537.36") ➞ "Google Chrome"

detectBrowser("Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:61.0) Gecko/20100101 Firefox/61.0") ➞ "Mozilla Firefox"

detectBrowser("Mozilla/5.0 (Windows NT 10.0; WOW64; Trident/7.0; .NET4.0C; .NET4.0E; .NET CLR 2.0.50727; .NET CLR 3.0.30729; .NET CLR 3.5.30729; rv:11.0) like Gecko") ➞ "Internet Explorer"
```
### :ramen:My Code
```js
let detectBrowser = userAgent => userAgent.includes("Firefox") ? "Mozilla Firefox" : userAgent.includes("Chrome") ? "Google Chrome" :
"Internet Explorer";
```
