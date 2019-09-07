## Volume of a Cone
Create a function that takes the height and radius of a cone as arguments and returns the volume of the cone. See the resources tab for the formula.

Volume of a Cone Image
```js
Examples
coneVolume(3, 2) ➞ 12.57

coneVolume(15, 6) ➞ 565.49

coneVolume(18, 0) ➞ 0
```
### :kaaba: My Code
```js
const coneVolume = (h,r) => +(Math.PI * r * r * h/3).toFixed(2);
```
