## Dashed Vowels

Create a function that takes a string and returns dashes on the left- and right side of every vowel ( A E I O U )
```
Examples
"Edabit" ➞ "-E-d-a-b-i-t"

"Carpe Diem" ➞ "C-a-rp-e- D-i--e-m"

"Fight for your right to party!" ➞ "F-i-ght f-o-r y-o--u-r r-i-ght t-o- p-a-rty!"

Notes:
A string can contain uppercase and lowercase vowels.
Y is not considered a vowel.
```
### :palm_tree: My Code
```js
const dashed = s => s.replace(/[aeiou]/gi,'-$&-');

//alternate
const dashed = s => [...s].map(a => /[aeiou]/gi.test(a) ? `-${a}-` : a).join('');
```
