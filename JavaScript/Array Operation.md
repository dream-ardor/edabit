## Array Operation

Create a function that takes three parameters and returns an array with the first parameter x, the second parameter y, and any number in between the first and second parameter in ascending order. Then filter through the array and return the array with numbers that are only divisible by the third parameter n.
```js
Examples
arrayOperation(1, 10, 3) ➞ [3, 6, 9]

arrayOperation(7, 9, 2) ➞ [8]

arrayOperation(15, 20, 7) ➞ []

Notes:
The final array should only consist of numbers between x and y inclusive that are divisible by n.
Return an empty array if there are no numbers that are divisible by n.
```
### :leaves: My Code
```js
const arrayOperation=(x,y,n)=> {
 let a = [];
  for(i=x; i<=y; i++) {if(i%n==0){a.push(i)}}
   return a;
}
```
