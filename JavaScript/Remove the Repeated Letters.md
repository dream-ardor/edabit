## remove the repeated letters

try to remove any repeated charcters in a word that will be passed to our function. any character could be used even special ones and numbers.
```js
Examples
unrepeated("hello")➞ "helo"

unrepeated("aaaaa")➞ "a"

unrepeated("WWE!!!") ➞ "WE!"

unrepeated("call 911") ➞ "cal 91"
```
### :computer: My Code
```js
let unrepeated = s => [...new Set(s)].join('');
```
