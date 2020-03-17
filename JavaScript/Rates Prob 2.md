## Rates Prob 2

If a person traveled up a hill for 18mins at 20mph and then traveled back down the same path at 60mph then their average speed traveled was 30mph.
```
Challenge
Write a function that returns the average speed traveled given an uphill time, uphill rate and a downhill rate
Uphill time is given in minutes
Return the rate as an integer (mph)
No rounding is necessary
aveSpd(18, 20, 60) ➞ 30 

Notes:
The solution is not dividing the sum of the speeds by 2
Check the Resources tab if your stuck
```
### :leaves: My Code
```js
const aveSpd = (ut, us, ds) => ds/2;
```
