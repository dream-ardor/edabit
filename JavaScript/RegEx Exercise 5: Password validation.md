RegEx Exercise 5: Password validation

```js
Create a regular expression that checks for a Password
- It should contain at least one uppercase letter
- It should contain at least one lowercase letter
- It should contain at least one digit
- It should contain at least one special symbol

REGEXP.test("bbA234c@cy~!")  ➞ true
REGEXP.test("32Bl4###xxz") ➞ true
REGEXP.test("!abcABC9lzD") ➞ true 
REGEXP.test("d@!2?%^&ahaZbb") ➞ true
```
### :computer: My Code
```js
const REGEXP = /[a-zA-Z\d\W]/
```
