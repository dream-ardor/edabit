## Reverse the Odd Length Words

Given a string, reverse all the words which have odd length. The even length words are not changed.
```js
Examples
reverseOdd("Bananas") ➞ "sananaB"

reverseOdd("One two three four") ➞ "enO owt eerht four"

reverseOdd("Make sure uoy only esrever sdrow of ddo length")
➞ "Make sure you only reverse words of odd length"
```
### :computer: My Code
```js
const reverseOdd = s => 
 s.split(' ').map(w => w.length % 2 ? [...w].reverse().join(''):w).join(' ');
```
