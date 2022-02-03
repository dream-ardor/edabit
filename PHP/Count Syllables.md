## Count Syllables

Create a function that counts the number of syllables a word has. Each syllable is separated with a dash -.
```php
Examples
numberSyllables("buf-fet") ➞ 2

numberSyllables("beau-ti-ful") ➞ 3

numberSyllables("mon-u-men-tal") ➞ 4

numberSyllables("on-o-mat-o-poe-ia") ➞ 6
```
### 🍃 My Code
```php
function numberSyllables($w) {
  return substr_count($w, "-") + 1;
}
```
