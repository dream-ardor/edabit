## Keyboard Mistakes

Character recognition software often makes mistakes when documents (especially old ones written with a typewriter) are digitized.

Your task is to correct the errors in the digitized text. You only have to handle the following mistakes:
```
A is misinterpreted as 4
S is misinterpreted as 5
O is misinterpreted as 0
I is misinterpreted as 1

The test cases contain numbers only by mistake.

Examples

keyboardMistakes("MUB45H1R") ➞ "MUBASHIR"

keyboardMistakes("DUBL1N") ➞ "DUBLIN"

keyboardMistakes("51NG4P0RE") ➞ "SINGAPORE"
```
### :leaves: My Code
```js
let keyboardMistakes = s => s.replace(/[4501]/g, a => a == 4 ? 'A' : a == 5 ? 'S': a == 0 ?  'O' : 'I');


//alternate solutions
const keyboardMistakes = txt => txt.replace(/\d/g, x => ["O", "I",,, "A", "S"][x]);

let keyboardMistakes = s => s.replace(/4/g,'A').replace('5','S').replace('1','I').replace('0','O');

function keyboardMistakes(txt) {
  let obj = { 4: "A", 5: "S", 0: "O", 1: "I" };
  return txt.replace(/\d/g, (x) => obj[x]);
}
```
