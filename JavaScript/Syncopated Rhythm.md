## Syncopated Rhythm

Syncopation means an emphasis on a weak beat of a bar of music; most commonly, beats 2 and 4 (and all other even-numbered beats if applicable).

s is a line of music, represented as a string, where hashtags # represent emphasized beats. Create a function that returns if the line of music contains any syncopation.
```js
Examples
hasSyncopation(".#.#.#.#") ➞ true

hasSyncopation("#.#...#.") ➞ false

hasSyncopation("#.#.###.") ➞ true
```
### :computer: My Code
```js
const hasSyncopation = s => [...s].some((e, i) => e === '#' && i % 2);

//regex
const hasSyncopation = s => !/^(.\.)*.?$/.test(s);

//alternate
const hasSyncopation = s => s.split('').map((a, i) => a === '#' ? i : -1).filter(i => i !== -1 && i % 2) .length > 0;

```
