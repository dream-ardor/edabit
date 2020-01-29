## Changing Mixed Types

Create a function which changes all the elements in an array as follows:
```
Add 1 to all even integers, nothing to odd integers.
Concatenates "!" to all strings and capitalises them.
Changes all boolean values to its opposite.
```
```js
Examples
change_types(["a", 12, True]) ➞ ["A!", 13, False]

change_types([13, "13", "12", "twelve"]) ➞ [13, "13!", "12!", "Twelve!"]

change_types([False, "False", "true"]) ➞ [True, "False!", "True!"]
```
### My Code
```js
const changeTypes = a =>
 a.map(b =>
  typeof b === 'string' ? b.charAt(0).toUpperCase() + b.slice(1) + '!' :
  typeof b === 'boolean' ? !b :
  b % 2 == 0 ? b + 1 : b);
```
