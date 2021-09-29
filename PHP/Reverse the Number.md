## Reverse the Number

Create a function that takes an integer $n and reverses it.
```php
Examples
rev(5121) ➞ "1215"

rev(69) ➞ "96"

rev(-122157) ➞ "751221"
```
### 🎋 My Code
```php
function rev($n) {
  return strrev((abs($n)));
}
```
