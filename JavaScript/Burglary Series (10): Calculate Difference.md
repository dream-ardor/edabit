## Burglary Series (10): Calculate Difference

The insurance guy calls again and apologizes. They found another policy made by your spouse, but this one is limited to cover a particular maximum in losses (for example, 50,000€). You send a bill to your spouse for the difference you lost.

Given an object of the stolen items and a limit, return the difference between the total value of those items and the limit of the policy.
```js
Examples
calculateDifference({ "baseball bat": 20 }, 5) ➞ 15

calculateDifference({ skate: 10, painting: 20 }, 19) ➞ 11

calculateDifference({ skate: 200, painting: 200, shoes: 1 }, 400) ➞ 1
```
### :leaves: My Code
```js
const calculateDifference = (o,l) => Object.values(o).reduce((a,b)=> a + b) - l;
```
