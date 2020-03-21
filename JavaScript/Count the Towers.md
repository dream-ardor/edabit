## Count the Towers

Create a function that counts the number of towers.
```js
Examples
count_towers([
  ["     ##         "],
  ["##   ##        ##"],
  ["##   ##   ##   ##"],
  ["##   ##   ##   ##"]
]) ➞ 4

count_towers([
  ["                         ##"],
  ["##             ##   ##   ##"],
  ["##        ##   ##   ##   ##"],
  ["##   ##   ##   ##   ##   ##"]
]) ➞ 6

count_towers([
  ["##"],
  ["##"]
]) ➞ 1

Notes:

You are given a 2D matrix.
Towers are two characters in length.
Towers are made only of the character #.
Some tests have no towers, return 0.
```
### :tokyo_tower: My Code
```js
const countTowers = T => T.pop()[0].split(/#+/).length - 1

//alternate
const countTowers = towers =>
  (towers[towers.length - 1][0].match(/##/g) || []).length;
  
//alternate
const countTowers = t => {
 let base = t[t.length - 1];
 return base[0].split(" ").filter(b => b.length === 2).length;
}
```
