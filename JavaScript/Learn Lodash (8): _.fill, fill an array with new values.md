## Learn Lodash (8): _.fill, fill an array with new values

According to the lodash documentation, _.fill Fills elements of an array with the value from start to, but not including, end. Note that this method mutates the array.
```
Arguments
array (Array): The array to fill.
value (*): The value to fill array with.
[start=0] (number): The start position.
[end=array.length] (number): The end position.
Returns
(Array): Returns array.
```
```js
Examples
var array = [1, 2, 3]

fill(array, "a") ➞ ["a", "a", "a"]

fill(Array(3), 2) ➞ [2, 2, 2]

fill([4, 6, 8, 10], "*", 1, 3) ➞ [4, "*", "*", 10]
```
### :palm_tree: My Code
```js
const fill = (a, v, s = 0, e = a.length) => a.fill(v,s,e);

```
