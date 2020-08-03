## A Long Long Time

Create a function that takes three values:
```
h hours
m minutes
s seconds

Return the value that's the longest duration.

Examples
longestTime(1, 59, 3598) ➞ 1

longestTime(2, 300, 15000) ➞ 300

longestTime(15, 955, 59400) ➞ 59400
```
### :sunny: My Code
```js
const longestTime = (h, m, s) => h < m/60 ? m < s/60 ? s : m : h;

```
