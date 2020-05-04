## Removing Enemies

Remove enemies from the list of people, even if the enemy shows up twice.
```js
Examples
removeEnemies(["Fred"], []) ➞ ["Fred"]

removeEnemies(["Adam", "Emmy", "Tanya", "Emmy"], ["Emmy"]) ➞ ["Adam", "Tanya"]

removeEnemies(["John", "Emily", "Steve", "Sam"], ["Sam", "John"]) ➞ ["Emily", "Steve"]
```
### :leaves: My Code
```js
const removeEnemies = (a,b) => a.filter(x => !b.includes(x));
```
