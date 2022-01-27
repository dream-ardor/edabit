## Find the Amount of Potatoes

Create a function to return the amount of potatoes there are in a string.
```php
Examples
potatoes("potato") ➞ 1

potatoes("potatopotato") ➞ 2

potatoes("potatoapple") ➞ 1
```
### 🥔  My Code
```php
function potatoes($s) {
  return substr_count($s,"to");
}
```
