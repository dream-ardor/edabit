## Check if the Same Case

Create a function that returns true if an input string contains only uppercase or only lowercase letters.
```
Examples
sameCase("hello") ➞ true

sameCase("HELLO") ➞ true

sameCase("Hello") ➞ false

sameCase("ketcHUp") ➞ false
```
### ↖️  My Code
```php
function sameCase($s) {
  return ctype_lower($s) || ctype_upper($s);
}
```
