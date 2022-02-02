## Calculate the % Difference between Two Numbers
Write a function that takes two integers as arguments and returns the percent difference between them.

The % difference between two numbers is the absolute value of the difference between the two numbers, divided by the average of those two numbers, multiplied by 100%.

% difference formula
```js
Examples
percentDiff(60, 100) ➞ 50.0

percentDiff(100, 60) ➞ 50.0

percentDiff(4538, 5439) ➞ 18.1

percentDiff(4538, 5439) ➞ 18.1
```
Notes
Round your result to one decimal place.
You will be given only whole numbers as test input.

### :dvd: My Code
```js
const percentDiff = (num1, num2) => +(Math.abs(num1 - num2) / ((num1+num2) / 2) * 100).toFixed(1);
```
