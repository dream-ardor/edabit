## Record Temperatures

You are given two arrays that each contain data that represents the min and max weather temperatures for each day of the week.

The records array contains the all-time record low/high temperatures for that day of the week.

[[record low, record high], ...]
The current week array contains the daily low/high temperatures for each day of the current week.

[[daily low, daily high], ...]
A daily high temperature is considered a new record high if it is higher than the record high for that day of the week. A daily low temperature is considered a new record low if it is lower than the record low for that day of the week.

Compare the daily low/high temperatures of the current week to the record lows/highs and return an array with the updated record temperatures.

There may be multiple record temperatures in a week.
If there are no broken records return the original records array.
```
Example
//             sun       mon      tues       wed      thur      fri       sat
recordTemps([[34, 82], [24, 82], [20, 89],  [5, 88],  [9, 88], [26, 89], [27, 83]],
            [[44, 72], [19, 70], [40, 69], [39, 68], [33, 64], [36, 70], [38, 69]])

➞           [[34, 82], [19, 82], [20, 89], [5, 88], [9, 88], [26, 89], [27, 83]]
The previous record low for Monday was 24. The current week's low for Monday was 19. So 19 replaces 24 as Monday's new record low.
```
### 🌡️  My Code
```js
let recordTemps = (a, b)=> a.map((c, d) => [Math.min(c[0], b[d][0]), Math.max(c[1], b[d][1])]);
```

