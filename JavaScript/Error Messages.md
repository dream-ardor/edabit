## Error Messages

Create a function that takes a number as an argument and returns the appropriate error message. You should do this without using the switch or if statements.

The input error will be 1 to 5:
```js
1 >> "Check the fan"
2 >> "Emergency stop"
3 >> "Pump Error"
4 >> "c"
5 >> "Temperature Sensor Error"

For any other value, return "101" (you can use an if statment here).

Examples
error(1) ➞ "Check the fan: e1"

error(2) ➞ "Emergency stop: e2"

error(3) ➞ "Pump Error: e3"
```
### My Code
```js
const error = n => {
 let a = {1: "Check the fan: e1",
 2: "Emergency stop: e2",
 3: "Pump Error: e3",
 4: "c: e4",
 5: "Temperature Sensor Error: e5"}
  return a[n] || 101;
}
```
