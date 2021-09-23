## Recursion: Length of a String

Write a function that returns the length of a string. Make your function recursive.
```php
Examples

length("apple") ➞ 5

length("make") ➞ 4

length("a") ➞ 1

length("") ➞ 0
```
### 💻 My Code
```php
function length($t) {
  return $t == '' ? 0:1 + strlen(substr($t, 1));
}

```
