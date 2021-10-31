## Broken Bridge

Create a function which validates whether a bridge is safe to walk on (i.e. has no gaps in it to fall through).
```
Examples
isSafeBridge("####") ➞ true

isSafeBridge("## ####") ➞ false

isSafeBridge("#") ➞ true
```
### 🌉 My Code
```php
function isSafeBridge($str) {
  return !strpos($str,' ');
}
```
