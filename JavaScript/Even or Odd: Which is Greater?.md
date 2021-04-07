## Even or Odd: Which is Greater?

Create a function to determine if the sum of all the individual even digits are greater than the sum of all the indiviudal odd digits in a string of numbers.

If the sum of odd numbers is greater than the sum of even numbers, return "Odd is greater than Even".
If the sum of even numbers is greater than the odd numbers, return "Even is greater than Odd".
If the sum of both even and odd numbers are equal, return "Even and Odd are the same".
```js
Examples

evenOrOdd("22471") ➞ "Even and Odd are the same"

evenOrOdd("213613") ➞ "Even and Odd are the same"

evenOrOdd("23456") ➞ "Even is greater than Odd"
```
### 🌻 My Code
```js
let evenOrOdd = s => {
  a = [...s].map(a => +a).filter(b => b % 2).reduce((a,b)=>a+b);
  b = [...s].map(a => +a).filter(b => !(b % 2)).reduce((a,b)=>a+b);
  return a > b ? 'Odd is greater than Even' : b > a ? 'Even is greater than Odd' : 'Even and Odd are the same';
}
```
