## Burglary Series (03): Is It Gone?

Your spouse is not concerned with the loss of material possessions but rather with his/her favorite pet. Is it gone?!

Given an object of the stolen items and a string in lower cases representing the name of the pet (e.g. "rambo"), return:

"Rambo is gone..." if the name is on the list.
"Rambo is here!" if the name is not on the list.
Note that the first letter of the name in the return statement is capitalized.
```js
Examples
const obj = {
  tv: 30,
  timmy: 20,
  stereo: 50,
} ➞ "Timmy is gone!"
// Timmy is in the object.


const obj = {
  tv: 30,
  stereo: 50,
} ➞ "Timmy is here!"
// Timmy is not in the stolen list object.

const obj = { } ➞ "Timmy is here!"
// Timmy is not in the object.
```
### :computer: My Code
```js
const findIt = (o,n) => o.hasOwnProperty(n) ? `${n.toUpperCase()[0] + n.slice(1)} is gone...` :
 `${n.toUpperCase()[0] + n.slice(1)} is here!`;


//alternate solution 1
const findIt = (obj, name) => {
 const displayName = name[0].toUpperCase() + name.slice(1);
 return `${displayName} is ${(name in obj) ? 'gone...' : 'here!'}`;
 
 //alternate solution 2
 const findIt = (obj, name) => `${name[0].toUpperCase()}${name.slice(1)} is ${name in obj ? "gone..." : "here!"}`;
};

//alternate solution 3
const findIt = (o, n, g = Object.keys(o).includes(n)) =>
 `${n[0].toUpperCase()}${n.slice(1)} is ${g ? `gone...` : `here!`}`;
```
