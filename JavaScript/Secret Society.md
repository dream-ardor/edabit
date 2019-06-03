## Secret Society

A group of friends have decided to start a secret society. The name will be the first letter of each of their names, sorted in alphabetical order.

Create a function that takes in an array of names and returns the name of the secret society.
```
Examples:
societyName(["Adam", "Sarah", "Malcolm"]) ➞ "AMS"

societyName(["Harry", "Newt", "Luna", "Cho"]) ➞ "CHLN"

societyName(["Phoebe", "Chandler", "Rachel", "Ross", "Monica", "Joey"]) ➞ "CJMPRR"
```
Notes:
The secret society's name should be entirely uppercased.

## My Code
```js
function societyName(friends) {
 let secret = friends.map((el) => el[0]).sort().join('');
 return secret;
}
```

## Analysis
We're creating a variable "secret" which utilizes the map function to iterate over each element of the friends parameter. Using arrow function, we take the first letter of each name (at index 0) and then chaining the sort function (to organize alphabetically) and the join function to combine the letters into a string. We use  ('') in the join function to remove whitespace and commas. Commas are the default separator when you don't supply an option, so we use '' to link them.
