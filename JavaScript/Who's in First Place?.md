## Who's in First Place?

Create a function that takes a string road and returns the car that's in first place. The road will be made of "=", and cars will be represented by letters in the alphabet.
```js
Examples

firstPlace("====b===O===e===U=A==") ➞ "A"

firstPlace("e==B=Fe") ➞ "e"

firstPlace("proeNeoOJGnfl") ➞ "l"
```
Notes:
Return "No car available" if there is no car on the road and "No road available" if there is no road.

### :palm_tree: My Code
```js
let firstPlace = r => (r.match(/[^=](?==*$)/) || [`No ${r ? "car" : "road"} available`])[0];


//alternate solutions
const firstPlace = r => r.replace(/=/g, '').slice(-1) || `No ${r ? 'car' : 'road' } available`;

const firstPlace = r => !r && 'No road available' || /\w/.test(r) && r.match(/\w/gi).pop() || 'No car available';

const firstPlace = r => r ? r.replace(/=/g,'').slice(-1)||'No car available':'No road available';
```
