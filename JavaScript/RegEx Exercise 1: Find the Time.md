## RegEx Exercise 1: Find the time

The time has a format: hours:minutes. Both hours and minutes has two digits, like 09:00.
```
Challenge:
- Make a regexp to find time in the string: Breakfast at 09:00 in the room 123:456.
- In this task there’s no need to check time correctness yet, so 25:99 can also be a valid result.
- The regexp should not match 123:456.
```
### :leaves: My Code
```js
const REGEXP = /\d{2}:\d{2}/
```
