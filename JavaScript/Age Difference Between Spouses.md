## Age Difference Between Spouses

Create a function that determines the age difference between spouses in a household. The ages ages in years of the parents and their children are given in an array.

If there is no difference in age between the parents, return 'No age difference between spouses'. Otherwise, return the difference in years. Check the examples for more clarifications.
```
Examples
ageDifference([29, 1, 6, 8, 28])  ➞ "1 year"

ageDifference([43, 86, 49, 86]) ➞  "No age difference between spouses."

iageDifference([2, 4, 6, 32, 27]) ➞ "5 years"

Notes
Note the singular 'year'.
The younger spouse (if the spouses are not the same age) will be older that their oldest kid by a minimum of 20 years.
The age difference be spouses will not be more than 18 years.
```
### :fallen_leaf: My Code
```js
const ageDifference = a => {
  let [d,e] = a.sort((b,c) => c - b), n = d - e;
  return n == 0 ? 'No age difference between spouses.': n > 1 ? `${n} years` : `1 year`;
}
```
