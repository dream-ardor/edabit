## Stuttering Function

Write a function that stutters a word as if someone is struggling to read it. The first two letters are repeated twice with an ellipsis ... and space after each, and then the word is pronounced with a question mark ?.
```js
Examples
stutter("incredible") ➞ "in... in... incredible?"

stutter("enthusiastic") ➞ "en... en... enthusiastic?"

stutter("outstanding") ➞ "ou... ou... outstanding?"
```
```
Notes:
Assume all input is in lower case and at least two characters long.
```
### :sunny: My Code
```js
const stutter = w =>`${w.slice(0,2)}... ${w.slice(0,2)}... ${w}?`;
```
