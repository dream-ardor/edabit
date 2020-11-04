## Hidden Calculator Words

At school, we used to play with our calculators and send each other secret messages. The trick was to enter a special number and turn the calculator upside-down. LOL ... I mean 707!

Given a number, create a function that converts it into a word by turning the integer 180 degrees around.
```js
Examples
turnCalc(707) ➞ "LOL"

turnCalc(5508) ➞ "BOSS"

turnCalc(3045) ➞ "SHOE"
```
### :palm_tree: My Code
```js
const turnCalc = n => {
  let a = 'OIZEHSGLB';
  return [...n+''].reverse().map(b => a[b]||'').join('');
}


//alternate solution
const turnCalc = n => [...n+''].map(a => a == '.' ? '' : a == '1' ? "I" :a == '2' ? 'Z' : a == '3' ? 'E' :
  a == '4' ? 'H' : a == '5' ? 'S' : a == '6' ? 'G' : a == '7' ? 'L' :
  a == '8' ? 'B' : 'O').reverse().join('');
```
