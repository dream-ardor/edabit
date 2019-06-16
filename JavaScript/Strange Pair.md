## Strange Pair

A pair of strings form a strange pair if:

1st string's first letter = 2nd string's last letter.
1st string's last letter = 2nd string's first letter.
Create a function that returns true if a pair of strings constitutes a strange pair, and false otherwise.
```js
Examples:

isStrangePair("ratio", "orator") ➞ true

// "ratio" ends with "o" and "orator" starts with "o".
// "ratio" starts with "r" and "orator" ends with "r".

isStrangePair("sparkling", "groups") ➞ true

isStrangePair("bush", "hubris") ➞ false

isStrangePair("", "") ➞ true
```

## My Code
```js
const isStrangePair = (str1, str2) => 
str1.charAt(0) == str2.slice(-1)
&&
str1.slice(-1) == str2.charAt(0);
```

## Analysis
An efficient way to solve this problem is to utilize a combination of the charAt and slice methods. The first part of my solution checks if the first character of string 1 is equivalent to the character at the end of string 2. The second part verifies that the inverse is true. Quick, simple and easy to read. :)
