## Broken Bridge

Create a function which validates whether a bridge is safe to walk on (i.e. has no gaps in it to fall through).
```js
Examples
isSafeBridge("####") ➞ true

isSafeBridge("## ####") ➞ false

isSafeBridge("#") ➞ true

Notes
You can expect the bridge's ends connecting it to its surrounding.
```
### :computer: My Code
```js
const isSafeBridge = s => !/\s/g.test(s);
```
