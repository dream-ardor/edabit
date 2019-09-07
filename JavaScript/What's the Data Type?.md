## What's the Data Type?
Create a function that returns the data type of a given variable. These are the eight data types this challenge will be testing for:
```
Array
Object
String
Number
Boolean
Null
Undefined
Date
```
```js
Examples
dataType([1, 2, 3, 4]) ➞ "array"

dataType({key: "value"}) ➞ "object"

dataType("This is an example string.") ➞ "string"

dataType(new Date()) ➞ "date"
```
### :kaaba: My Code
```js
const dataType = v =>
 v ? v.constructor.name.toLowerCase() : String(v);
```
