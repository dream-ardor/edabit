## Fix The Spacing
Additional spaces have been added to a sentence. Return the correct sentence by removing them. All words should be separated by one space, and there should be no spaces at the beginning or end of the sentence.
```js
Examples
correctSpacing("The film   starts       at      midnight. ")
➞ "The film starts at midnight."

correctSpacing("The     waves were crashing  on the     shore.   ")
➞ "The waves were crashing on the shore."

correctSpacing(" Always look on    the bright   side of  life.")
➞ "Always look on the bright side of life."
```
### :small_blue_diamond:My Code
```js
const correctSpacing = s => s.replace(/\s+/g, ' ').trim();
```

## Recursion: String Palindromes
Write a function that recursively determines if a string is a palindrome.
```js
Examples
isPalindrome("abcba") ➞ true

isPalindrome("b") ➞ true

isPalindrome("") ➞ true

isPalindrome("ad") ➞ false
```
### :small_blue_diamond:My Code
```js
const isPalindrome = str => {
    const str1 = str.length;
    if (str1 < 2) {
        return true;
    }

    if (str[0] === str[str1 - 1]) {
        return isPalindrome( str.slice(1, str1 - 1) );
    }

    return false;
};
```

## Check for Anagrams
Create a function that takes two strings and returns (true or false) whether they're anagrams or not.
```js
Examples
isAnagram("cristian", "Cristina") ➞ true

isAnagram("Dave Barry", "Ray Adverb") ➞ true

isAnagram("Nope", "Note") ➞ false
```

### :small_blue_diamond:My Code
```js
//checks for whitespaces and non-alphanumeric characters
const isAnagram = (a,b) => {
    let c = a.replace(/\W+/g, '').toLowerCase().split("").sort().join("");
    let d = b.replace(/\W+/g, '').toLowerCase().split("").sort().join("");
    return c === d  ? true : false;
}

//shortened
const isAnagram = (a,b) => 
a.toLowerCase().split('').sort().join('') ===
b.toLowerCase().split('').sort().join('')


```

## Basic E-Mail Validation
Create a function that accepts a string, checks if it's a valid email address and returns either true or false, depending on the evaluation.
```js
The string must contain an @ character.
The string must contain a . character.
The @ must have at least one character in front of it.
e.g. "e@edabit.com" is valid while "@edabit.com" is invalid.
The . and the @ must be in the appropriate places.
e.g. "hello.email@com" is invalid while "john.smith@email.com" is valid.
If the string passes these tests, it's considered a valid email address.
```
```js
Examples
validateEmail("@gmail.com") ➞ false

validateEmail("hello.gmail@com") ➞ false

validateEmail("gmail") ➞ false

validateEmail("hello@gmail") ➞ false

validateEmail("hello@edabit.com") ➞ true
```
### :small_blue_diamond:My Code
```js
const validateEmail = str =>  str.indexOf("@") > 0 && str.includes(".com");
```
## Is the Phone Number Formatted Correctly?
Create a function that accepts a string and returns true if it's in the format of a proper phone number and false if it's not. Assume any number between 0-9 (in the appropriate spots) will produce a valid phone number. This is what a valid phone number looks like: (123) 456-7890
```js
Examples
isValidPhoneNumber("(123) 456-7890") ➞ true

isValidPhoneNumber("1111)555 2345") ➞ false

isValidPhoneNumber("098) 123 4567") ➞ false
```
### :small_blue_diamond:My Code
```js
const isValidPhoneNumber = str => /^\(\d{3}\)\s\d{3}-\d{4}$/.test(str);
```

## Return an Array of Subarrays
Write a function that takes three arguments (x, y, z) and returns an array containing subarrays (e.g. [[], [], []]), each of a certain number of items, all set to either a string or an integer.

x argument: Number of subarrays contained within the main array.
y argument Number of items contained within each subarray(s).
z argument: Item contained within each subarray(s).
```js
Examples
matrix(3, 2, 3) ➞ [[3, 3], [3, 3], [3, 3]]

matrix(2, 1, "edabit") ➞ [["edabit"], ["edabit"]]

matrix(3, 2, 0) ➞ [[0, 0], [0, 0], [0, 0]]
```
### :small_blue_diamond:My Code
```js
//using fill method
const matrix = (x, y, z) => Array(x).fill(Array(y).fill(z));

//using for loop
function matrix(x, y, z) {
  let a = [];
   for (i = 0; i < x; i++) {
    a.push([])
   for (j = 0; j < y; j++){
    a[i].push(z)
 }
}
  return a;
}
```




