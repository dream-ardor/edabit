## Western Showdown

Wild Roger is participating in a Western Showdown, meaning he has to draw (pull out and shoot) his gun faster than his opponent in a gun standoff.

Given two strings,p1 and p2, return which person drew their gun the fastest. If both are drawn at the same time, return 'tie'.
```js
Examples
showdown(
'   Bang!        ',
'        Bang!   '
) ➞ 'p1'
 // p1 draws his gun sooner than p2


showdown(
'               Bang! ',
'             Bang!   '
) ➞ 'p2'


showdown(
'     Bang!   ',
'     Bang!   '
) ➞ 'tie'
```
### :leaves: My Code
```js
const showdown = (p1, p2) => 
 p1.indexOf('B') < p2.indexOf('B') ? 'p1' :
 p2.indexOf('B') < p1.indexOf('B') ? 'p2' : 'tie';
```
