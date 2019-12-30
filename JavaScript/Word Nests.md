## Word Nests

A word nest is created by taking a starting word, and generating a new string by placing the word inside itself. This process is then repeated.

Nesting 3 times with the word "incredible":
```js
start  = incredible
first  = incre|incredible|dible
second = increin|incredible|credibledible
third  = increinincr|incredible|ediblecredibledible
```
The final nest is "increinincrincredibleediblecredibledible" (depth = 3).

Given a starting word and the final word nest, return the depth of the word nest.
```js
Examples
wordNest("floor", "floor") ➞ 0

wordNest("code", "cocodccococodededeodeede") ➞ 5

wordNest("incredible", "increinincrincredibleediblecredibledible") ➞ 3
```
### :leaves: My Code
```js
const wordNest = (w,n) => n.length / w.length - 1;
```
