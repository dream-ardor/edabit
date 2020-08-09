## Musical Cadences

In music, cadences act as punctuation in musical phrases, and help to mark the end of phrases. Cadences are the two chords at the end of a phrase. The different cadences are as follows:
```
V followed by I is a Perfect Cadence
IV followed by I is a Plagal Cadence
V followed by Any chord other than I is an Interrupted Cadence
Any chord followed by V is an Imperfect Cadence
Create a function where given a chord progression as an array, return the type of cadence the phrase ends on.

Examples
findCadence(["I", "IV", "V"]) ➞ "imperfect"

findCadence(["ii", "V", "I"]) ➞ "perfect"

findCadence(["I", "IV", "I", "V", "vi"]) ➞ "interrupted"

Notes:
Return strings all in lowercase.
Only focus on the last two chords of a progression.
Return "no cadence" if none of the criterea match up.
I is a capital i not a lowercase L.
```
### :notes: My Code
```js
const findCadence = c => c.slice(-2).join('') == 'IVI' ? 'plagal' : c.slice(-2).join('') == 'VI' ? 'perfect' : 
 c[c.length-1] == 'V' ? 'imperfect' : c[c.length-2] == 'V' &&  c[c.length-1] !== 'I' ? 'interrupted' : 'no cadence';
```
