## Human, Cat and Dog Years 🧑🏻🐱🐶

Mubashir has a cat and a dog. He purchased both of them at the same time Human Years ago.

Create a function which takes an argument of humanYears and returns [humanYears, catYears, dogYears] array.
```
Human Years
Human Years >= 1
Human Years are whole numbers only.

Cat Years
15 cat years for first year.
+9 cat years for second year.
+4 cat years for each year after that.

Dog Years
15 dog years for first year
+9 dog years for second year
+5 dog years for each year after that

Examples
calculateYears(1) ➞ [1, 15, 15]

calculateYears(2) ➞ [2, 24, 24]

calculateYears(10) ➞ [10, 56, 64]
```
### My Code
```js
const calculateYears = h => h == 1 ? [1,15,15] : [h,(h + 4) * 4, (h * 5) + 9 + 5];

//alternate solution
const calculateYears = h => {
  let a = [h,15,15];
  for (let i = 1; i < h; i++) {
   if (i == 1) a[1] +=9, a[2] +=9;
   else a[1] +=4, a[2] +=5;
 }
  return a;
}
```
