## Repeat the Same Item Multiple Times

Create a function that takes two arguments (item, times). The first argument (item) is the item that needs repeating while the second argument (times) is the number of times the item is to be repeated. Return the result in an array.
```php
Examples
repeat("edabit", 3) ➞ ["edabit", "edabit", "edabit"]

repeat(13, 5) ➞ [13, 13, 13, 13, 13]

repeat("7", 2) ➞ ["7", "7"]

repeat(0, 0) ➞ []
```
### 🔁 My Code
```php
function repeat($i, $t){
  return array_fill(0, $t, $i);
}
```
