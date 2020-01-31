## Enharmonic Equivalents

In music, notes can be written out in multiple ways (especially for notes on the black keys). Although these notes are spelled out differently, they still are the same note physically.
```
C# = Db, D# = Eb, F# = Gb, G# = Ab, A# = Bb
```
Given a musical note, create a function that returns its enharmonic equivalent. The examples below should make this clear.
```js
Examples
getEquivalent("D#") ➞ "Eb"

getEquivalent("Gb") ➞ "F#"

getEquivalent("Bb") ➞"A#"
```
### :musical_note: My Code
```js
const getEquivalent = n => {
 switch(n) {
	case 'C#': return 'Db'; break;
	case 'Db': return "C#"; break;
	case 'D#': return 'Eb'; break;
	case 'Eb': return 'D#'; break;
  case 'F#': return 'Gb'; break;
	case 'Gb': return 'F#'; break;
	case 'G#': return 'Ab'; break;
	case 'Ab': return 'G#'; break;
	case 'A#': return 'Bb'; break;
	case 'Bb': return 'A#'		
 };
}
```
