## One Odd and One Even

Given a two digit number, return true if that number contains one even and one odd digit.
```js
Examples
oneOddOneEven(12) ➞ true

oneOddOneEven(55) ➞ false

oneOddOneEven(22) ➞ false
```
### :computer: My Code
```js
const oneOddOneEven = n => 
 +String(n)[0] % 2 != +String(n)[1] % 2;
```
