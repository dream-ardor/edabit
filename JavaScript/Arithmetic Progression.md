## Arithmetic Progression

In mathematics, an Arithmetic Progression (AP) is a sequence of numbers such that the difference between the consecutive terms is constant. Create a function that takes three arguments:
```
First element of the sequence first
Constant difference between the elements diff
Total numbers in the sequence n
Return the first n elements of the sequence with the given common difference diff. The final result should be a string of numbers, separated by comma and space.
```
```js
Examples
arithmeticProgression(1, 2, 5) ➞ "1, 3, 5, 7, 9"

arithmeticProgression(1, 0, 5) ➞ "1, 1, 1, 1, 1"

arithmeticProgression(1, -3, 10) ➞ "1, -2, -5, -8, -11, -14, -17, -20, -23, -26"
```
### 🏜️ My Code
```js
const arithmeticProgression = (s,d,n) => [...Array(n)].map((_,i)=> s + i * d).join(', ');


//alternate solutions
constt arithmeticProgression = (a, b, n) => {
  let arr = [];
  let i = 0;
   while(i < n) {arr.push(a);
    a += b;
    i += 1;}
  return arr.join(', ');}
  
  
const arithmeticProgression = (s, d, n) => Array.from({length: n}, (_,i) => s + d * i).join(', ');
```
