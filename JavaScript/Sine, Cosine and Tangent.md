## Sine, Cosine and Tangent

Create three functions that will do three things:
```js
Multiply one number by the sine of another number.
Multiply one number by the COSINE of another number.
Multiply one number by the tangent of another number.
In each function, you will be given 2 numbers: x and y. Another important thing to note, the numbers will be in degrees, not radians. That is extremely important. Remember to round the result to 2 decimal places, as well.

Examples
sine(8, 27) ➞ 8 sin 27 ➞ 3.63

cosine(10, 4) ➞ 10 cos 4 ➞ 0.70

tangent(4, 39) ➞ 4 tan 39 ➞ 2.52
```
### :leaves: My Code
```js
const sine = (x,y) => +(x * Math.sin(y * Math.PI / 180)).toFixed(2);
const cosine = (x,y) => +(x * Math.cos(y * Math.PI / 180)).toFixed(2);
const tangent = (x,y) => +(x * Math.tan(y * Math.PI / 180)).toFixed(2);
```
