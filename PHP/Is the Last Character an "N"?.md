## Is the Last Character an "N"?

Create a function that takes a string (a random name). If the last character of the name is an "n", return true, otherwise return false.
```php
Examples
isLastCharacterN("Aiden") ➞ true

isLastCharacterN("Piet") ➞ false

isLastCharacterN("Bert") ➞ false

isLastCharacterN("Dean") ➞ true
```
### ❔ My Code
```php
function isLastCharacterN($w) {
  return substr($w, -1) == "n";
}
```
