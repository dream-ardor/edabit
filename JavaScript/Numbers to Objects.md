## Numbers to Objects
```
Mubashir needs your help in a simple task.

Given an array of numbers arr:

Create an object against each given number.
The object key will be the number converted string.
The value will be the corresponding character code converted string (check ASCII table).
Return an array of the resulting objects.

Examples

numObj([118, 117, 120]) ➞ [{'118':'v'}, {'117':'u'}, {'120':'x'}]

numObj([101, 121, 110, 113, 103]) ➞ [{'101':'e'}, {'121':'y'}, {'110':'n'}, {'113':'q'}, {'103':'g'}]

numObj([118, 103, 110]) ➞ [{"118":"v"}, {"103":"g"}, {"110":"n"}
```
### 🌴 My Code
```js
const numObj = a => a.map(x=>({[x]:String.fromCharCode(x)}));
```
