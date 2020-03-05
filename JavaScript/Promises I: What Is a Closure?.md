## Promises I: What Is a Closure?

Closures are functions that remember their lexical environments. Lexical environments mean the environment in which the function was declared.
```js
function parent(x) {
  return function closure() {    // Closure is declared here.
    return x
  }
}

const remember = parent("remembers me")
// Seems like the variable x would be gone after
// parent is executed, but it's not.

closure()
// Returns "remembers me" because the inner
// function remembers x.
```
Fix the greetingMaker() function so that it works with the greeting() function.
The greeting() function has already been created (check the Tests tab).
```js
Example
const greeting = greetingMaker("Hello")
greeting("James") ➞ "Hello, James"
```
### :computer: My Code
```js
const greetingMaker = n => g => `${n}, ${g}`;
```
