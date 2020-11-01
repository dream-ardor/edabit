## Calculating Damage

Create a function that takes damage and speed (attacks per second) and returns the amount of damage after a given time.
```js
Examples
damage(40, 5, "second") ➞ 200

damage(100, 1, "minute") ➞ 6000

damage(2, 100, "hour") ➞ 720000

Notes:
Return "invalid" if damage or speed is negative.
```
### :jack_o_lantern: My Code
```js
const damage = (d,s,t) => d < 0 || s < 0 ? 'invalid': t == 'second' ? d*s : t == 'minute' ? d*s*60 : d*s*3600;
```
