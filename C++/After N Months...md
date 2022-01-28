## After N Months...

Create a function that takes in year and months as input, then return what year it would be after n-months has elapsed.
```
Examples
afterNMonths(2020, 24) ➞ 2022

afterNMonths(1832, 2) ➞ 1832

afterNMonths(1444, 60) ➞ 1449
```

### 🗓️ My Code
```c++
#define afterNMonths(y, m) y + m / 12
```
