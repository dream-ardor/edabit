## Valid Variable Names

When creating variables, the variable name must always start with a letter, though numbers and underscores are allowed to be contained in it also.

Create a function which returns true if a given variable name is valid, otherwise return false.
```js
Examples
variableValid("result") ➞ true

variableValid("odd_nums") ➞ true

variableValid("2TimesN") ➞ false
```
### :capital_abcd: My Code
```js
const variableValid = v => /^[a-z]\S+$/.test(v);
```
