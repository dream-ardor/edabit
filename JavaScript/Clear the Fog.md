## Clear the Fog

Create a function which returns the word in the string, but with all the fog letters removed. However, if the string is clear from fog, return "It's a clear day!".
```js
Examples
clearFog("sky") ➞ "It's a clear day!"

clearFog("fogfogfffoooofftreesggfoogfog") ➞ "trees"

clearFog("fogFogFogffffooobirdsandthebeesGGGfogFog") ➞ "birdsandthebees"
```
### :evergreen_tree: My Code
```js
const clearFog = s => !/fog/g.test(s) ? "It's a clear day!" :
 s.replace(/[fog]/g, '');
```
