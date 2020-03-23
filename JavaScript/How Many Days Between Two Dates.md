## How Many Days Between Two Dates

Create a function that takes two dates and returns the number of days between the first and second date.
```js
Examples
getDays(
  new Date("June 14, 2019"),
  new Date("June 20, 2019")
) ➞ 6

getDays(
  new Date("December 29, 2018"),
  new Date("January 1, 2019")
) ➞ 3

getDays(
  new Date("July 20, 2019"),
  new Date("July 30, 2019")
) ➞ 10
```
### :calendar: My Code
```js
const getDays = (d1,d2) =>
 Math.round(Math.abs(d1-d2) / 8.64e7);
```
