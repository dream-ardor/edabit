The Fizz Buzz Test

The Fizz Buzz test is a poplular interview question used to 'help filter out the 99.5% of programming job candidates who can't seem to program their way out of a wet paper bag.'

Write a program that returns array of all the numbers from 1 to an interger argument. But for multiples of three use “Fizz” instead of the number and for the multiples of five use “Buzz”. For numbers which are multiples of both three and five use “FizzBuzz”
```js
Example
fizzBuzz(10) ➞ [1, 2, 'Fizz', 4, 'Buzz', 'Fizz', 7, 8, 'Fizz', 'Buzz']

fizzBuzz(15) ➞ [1, 2, 'Fizz', 4, 'Buzz', 'Fizz', 7, 8, 'Fizz', 'Buzz', 11, 'Fizz', 13, 14, 'FizzBuzz']

Notes:
Make sure to return array.
```
### :leaves: My Code
```js
const fizzBuzz = n => [...Array(n)].map((v,i)=>i+1).map(x=>
 x % 15 == 0 ? 'FizzBuzz':
 x % 3 == 0 ? 'Fizz':
 x % 5 == 0 ? 'Buzz': x);
```
