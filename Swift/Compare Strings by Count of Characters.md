## Compare Strings by Count of Characters

Create a function that takes two strings as arguments and return either true or false depending on whether the total number of characters in the first string is equal to the total number of characters in the second string.
```php
Examples
comp("AB", "CD") ➞ true

comp("ABC", "DE") ➞ false

comp("hello", "edabit") ➞ false
```
### ➗ My Code
```php
function comp($a, $b) {
  return strlen($a) == strlen($b);
}
```
