## Fullname and Email

Create the instance properties fullname and email in the Employee class. Given a person's first and last names:
```js
Form the fullname by simply joining the first and last name together, separated by a space.
Form the email by joining the first and last name together with a . in between, and follow it with @company.com at the end. Make sure everything is in lowercase.

Examples
emp1 = Employee('John', 'Smith')
emp1.fullname ➞ 'John Smith'

emp2 = Employee('Mary',  'Sue')
emp2.email ➞ 'mary.sue@company.com'

emp3 = Employee('Antony', 'Walker')
emp3.firstname ➞ 'Antony'
```
### :leaves: My Code
```js
class Employee {
 constructor (fn, ln) {
  this.firstname = fn;
  this.lastname = ln;
  this.fullname = fn + ' ' + ln;
  this.email = fn.toLowerCase() + '.' + ln.toLowerCase() + '@company.com'.toLowerCase();
	}
}
```
