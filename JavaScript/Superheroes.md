## Superheroes

Create a function that takes an array of Superheroes and Superheroines names and returns an array of only superheroes names that are ending in "man". Return them in alphabetical order.

Wonder-Woman, Catwoman and Invisible-Woman are Superheroines, not Superheroes. Return only Superheroes.
```js
Examples
["Batman", "Superman", "Spider-man", "Hulk", "Wolverine", "Wonder-Woman"] ➞ ["Batman", "Spider-man", "Superman"]

["Wonder-Woman", "Catwoman", "Invisible-Woman"] ➞ []

["Catwoman", "Deadpool", "Dr.Strange", "Captain-America", "Aquaman", "Hawkeye"] ➞ ["Aquaman"]
```
### :leaves: My Code
```js
const superheroes = h => h.filter(a => a.match(/[^wo]man$/g)).sort();
```
