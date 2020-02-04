## Skip the Drinks with Too Much Sugar

The function skipTooMuchSugarDrinks() takes in an array of drinks. Make sure the function only returns an array of drinks with no sugar in it or a little bit of sugar.

Drinks that contain too much sugar (in this challenge) are:
```
Cola
Fanta
```
```js
Examples
skipTooMuchSugarDrinks(["fanta", "cola", "water"]) ➞ [water]

skipTooMuchSugarDrinks(["fanta", "cola"]) ➞ []

skipTooMuchSugarDrinks(["lemonade", "beer", "water"]) ➞ ["lemonade", "beer", "water"]
```
### :fallen_leaf: My Code
```js
const skipTooMuchSugarDrinks = d =>
  d.filter(x=> x !== 'cola' && x !== 'fanta');
```
