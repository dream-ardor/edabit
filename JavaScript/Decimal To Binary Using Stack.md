## Decimal To Binary Using Stack

Create a function that takes a decimal number and converts into binary number using Stack.The Stack is created for you.
```js
Examples
toBinary(12) ➞ 1100

toBinary(0) ➞ 0

toBinary(101) ➞ 1100101

Notes
0 <= n <= 101
```
### :sunny: My Code
```js
function Stack() {
  let data = [];
  this.push = function (item) {
    data.push(item);
  };
  this.isEmpty = function () {
    return !data.length;
  };
  this.pop = function () {
    return data.pop();
  };
  this.peek = function () {
    return data[data.length - 1];
  };
  this.size = function () {
    return data.length;
  };
}


function toBinary(n){
  let stack = new Stack();
  return +(n >>> 0).toString(2);
}
```
