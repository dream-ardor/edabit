## Free Coffee Cups

For each of the 6 coffee cups I buy, I get a 7th cup free. In total, I get 7 cups. Create a function that takes n cups bought and return the total number of cups I would get.
```php
Examples
total_cups(6) ➞ 7

total_cups(12) ➞ 14

total_cups(213) ➞ 248
```
### ☕  My Code
```php
function total_cups ($n) {
  return $n * 7 / 6 || 0;
}
```
