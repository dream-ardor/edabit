## Return the End Letters of Numbers

Create a function that takes an integer and returns it as an ordinal number. An Ordinal Number is a number that tells the position of something in a list, such as 1st, 2nd, 3rd, 4th, 5th etc.
```js
Examples
returnEndOfNumber(553) ➞ "553-RD"

returnEndOfNumber(34) ➞ "34-TH"

returnEndOfNumber(1231) ➞ "1231-ST"

returnEndOfNumber(22) ➞ "22-ND"
```
### :fallen_leaf: My Code
```js
const returnEndOfNumber = n => {
  let a = ["TH","ST","ND","RD"],
      b = n % 100;
  return n + '-' +(a[(b-20)%10]||a[b]||a[0]);
}
```
