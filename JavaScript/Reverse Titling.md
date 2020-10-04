## Reverse Titling

Your stereotypical titleCase() function in JavaScript might capitalises the first letter of every word in a given sentence, leaving all the other letters as lowercase.

The goal of this challenge, however, is to create a reverseTitle() function, which achieves the complete opposite! Make the first letter of every word lowercase, and the rest uppercase!
```js
Examples
reverseTitle("this is a title") ➞ "tHIS iS a tITLE"

reverseTitle("BOLD AND BRASH!") ➞ "bOLD aND bRASH!"

reverseTitle("Elephants dance about bravely in Thailand") ➞ "eLEPHANTS dANCE aBOUT bRAVELY iN tHAILAND"
```
### :computer: My Code
```js
const reverseTitle = s => s.replace(/(^\w|\s\w)(\S*)/g, (_,a,b) => a.toLowerCase()+b.toUpperCase());


//alternate solutions

const reverseTitle = s => s.toUpperCase().replace(/^.| ./g,(c)=>c.toLowerCase());

const reverseTitle = s => s.toUpperCase().split(' ').map(a => a.charAt(0).toLowerCase() + a.slice(1)).join(' ');

const reverseTitle = s => (s.replace(/\w+?(?=\b)/g, m => (m[0].toLowerCase() + m.slice(1).toUpperCase())));

```
