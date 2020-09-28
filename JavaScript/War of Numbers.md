## War of Numbers

There's a great war between the even and odd numbers. Many numbers already lost their life in this war and it's your task to end this. You have to determine which group is larger: the even, or the odd. The larger group wins.

Create a function that takes an array of integers, sums the even and odd numbers seperately, then returns the larger of the sums minus the smaller.
```js
Examples
warOfNumbers([2, 8, 7, 5]) ➞ 2
// 2 + 8 = 10
// 7 + 5 = 12
// 12 is larger than 10
// So we return 12 - 10 = 2

warOfNumbers([12, 90, 75]) ➞ 27

warOfNumbers([5, 9, 45, 6, 2, 7, 34, 8, 6, 90, 5, 243]) ➞ 168
```
### :palm_tree:	My Code
```js
const warOfNumbers = a => Math.abs(a.reduce((b,c)=> c % 2 == 0 ? b+c : b-c,0));

//alternate
const warOfNumbers = a => {
 let a1  = a.filter(n => n % 2 ).reduce((b,c) => b + c);
 let b1 = a.filter(n => n % 2 == 0).reduce((b,c) => b + c);
 return a1 > b1 ? a1 - b1 : b1 - a1;
};
```
