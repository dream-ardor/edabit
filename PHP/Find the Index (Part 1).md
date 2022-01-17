# Find the Index (Part 1)

Create a function that finds the index of a given item.
```php
Examples
search([1, 5, 3], 5) ➞ 1

search([9, 8, 3], 3) ➞ 2

search([1, 2, 3], 4) ➞ -1
```
### 🗳️ My Code
```php
function search($a,$i) {
  return in_array($i,$a) || -1;
}
```
