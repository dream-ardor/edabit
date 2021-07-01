## Return the Four Letter Strings

Create a function that takes an array of strings and returns the words that are exactly four letters.
```php
Examples

isFourLetters(["Tomato", "Potato", "Pair"]) ➞ ["Pair"]

isFourLetters(["Kangaroo", "Bear", "Fox"]) ➞ ["Bear"]

isFourLetters(["Ryan", "Kieran", "Jason", "Matt"]) ➞ ["Ryan", "Matt"]
```
### 💻 My Code
```php
function isFourLetters($a) {
  return array_values(array_filter($a, function ($b) {return strlen ($b) == 4;}));
}
```
