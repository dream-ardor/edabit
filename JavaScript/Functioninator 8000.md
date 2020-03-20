## Functioninator 8000

Create a function that takes a single word string and does the following:

Concatenates inator to the end if the word ends with a consonant otherwise, concatenate -inator instead.

Adds the word length of the original word to the end, supplied with '000'.

The examples should make this clear.
```js
Examples
inatorInator("Shrink") ➞ "Shrinkinator 6000"

inatorInator("Doom") ➞ "Doominator 4000"

inatorInator("EvilClone") ➞ "EvilClone-inator 9000"
```
### My Code
```js
let inatorInator = s =>
  `${s+(/[aeio]$/i.test(s)?'-':'')}inator ${s.length}000`
```
