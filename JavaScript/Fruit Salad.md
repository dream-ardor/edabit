## Fruit Salad 🍇🍓🍎

Fruit salads are served best when the fruits are sliced and diced into small chunks!

For this challenge, slice each fruit in half and sort the chunks alphabetically. This recipe tastes best when the chunks are joined together to make a string.
```js
Worked Example
fruitSalad(['apple', 'pear', 'grapes']) ➞ 'apargrapepesple'

# Chunks: ['ap', 'ple', 'pe', 'ar', 'gra', 'pes']
# Sorted chunks: ['ap', 'ar', 'gra', 'pe', 'pes', 'ple']
# Final string: 'apargrapepesple'

Examples
fruitSalad(['apple', 'pear', 'grapes']) ➞ 'apargrapepesple'

fruitSalad(['raspberries', 'mango']) ➞ 'erriesmangoraspb'

fruitSalad(['banana']) ➞ 'anaban'

Notes:
If a fruit has an odd number of letters, make the right side larger than the left.
For example: 'apple' will be sliced into 'ap' and 'ple'.
All fruits will be given in lowercase.
```
### :cactus: My Code
```js
const fruitSalad = a => a.flatMap(b => [b.slice(0,b.length/2),b.slice(Math.floor(b.length/2,0))]).sort().join('');

//alternate solution
const fruitSalad = a =>  {
  let c = a.map(b => b.slice(Math.floor(b.length/2)));
  let d = a.map(b => b.slice(0,b.length/2));
  return [c,d].flat().sort().join('');
}
```
