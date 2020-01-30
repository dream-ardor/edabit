## Hello; Hello World; World

Write a function that takes an integer and:
```
If the number is a multiple of 3, return "Hello".
If the number is a multiple of 5, return "World".
If the number is a multiple of both 3 and 5, return "Hello World".
```
```js
Examples
helloWorld(3) ➞ "Hello"

helloWorld(5) ➞ "World"

helloWorld(15) ➞ "Hello World"
```
### :computer: My Code
```js
const helloWorld = n => n % 3 == 0 && n % 5 == 0 ? "Hello World" :
 n % 3 == 0 ? "Hello" : "World";

```
