## The Full Length of a Google

Google's logo can be stretched depending on how many pages it lets you skip forward to.

Image of Goooooooooogle

Let's say we wanted to change the number of pages that Google could skip to. Create a function where given a number of pages $n, return the word "Google" but with the correct number of "o"s.
```
Examples
googlify(10) ➞ "Goooooooooogle"

googlify(23) ➞ "Gooooooooooooooooooooooogle"

googlify(2) ➞ "Google"

googlify(-2) ➞ "invalid"
```
### 🏜️ My Code
```php
function googlify($n) {
  return $n < 2 ? "invalid" : "G" . str_repeat("o",$n) . "gle";
}
```
