## Temperature Conversion

Write a program that takes a temperature input in celsius and converts it to Fahrenheit and Kelvin. Return the converted temperature values in an array.

The formula to calculate the temperature in Fahrenheit from Celsius is:
```
F = C*9/5 +32
The formula to calculate the temperature in Kelvin from Celsius is:

K = C + 273.15

Examples
tempConversion(0) ➞ [32, 273.15]
// 0°C is equal to 32°F and 273.15 K.

tempConversion(100) ➞ [212, 373.15]

tempConversion(-10) ➞ [14, 263.15]

tempConversion(300.4) ➞ [572.72, 573.55]
```
### :computer: My Code
```js
const tempConversion = c => c > -273.15 ? [+(c*9/5 +32).toFixed(2), +(c+273.15).toFixed(2)] : 'Invalid';


//alternate solution
const tempConversion = c =>  
 [+(c*9/5 + 32).toFixed(2) ,+(c + 273.15).toFixed(2)][1] < 0 ? 'Invalid':
 [+(c*9/5 + 32).toFixed(2) ,+(c + 273.15).toFixed(2)];
```
