## Moving House

I'd like to calculate how long on average I've lived in a single house.

Given a person's age and the number of times they've moved house as moves, return the average number of years that they've spent living in the same house.
```js
Examples
yearsInOneHouse(30, 1) ➞ 15

yearsInOneHouse(15, 2) ➞ 5

yearsInOneHouse(80, 0) ➞ 80
```
### :evergreen_tree: My Code
```js
const yearsInOneHouse = (a, m) => Math.round(a / (m + 1));
```
