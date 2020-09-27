## Name Classes

Write a class called Name and create the following attributes given a first name and last name (as fname and lname):

- An attribute called fullname which returns the first and last names.
- A attribute called initials which returns the first letters of the first and last name. Put a . between the two letters.
- Remember to allow the attributes fname and lname to be accessed individually as well.
```js
Examples
a1 = new Name("john", "SMITH")
a1.fname ➞ "John"

a1.lname ➞ "Smith"

a1.fullname ➞ "John Smith"
```
### :computer: My Code
```js
class Name {
 constructor(a, b) {
  this.fname = a[0].toUpperCase()+a.slice(1).toLowerCase();
  this.lname = b[0].toUpperCase()+b.slice(1).toLowerCase();
  this.fullname = this.fname + ' ' + this.lname;
  this.initials = this.fname[0] + '.' + this.lname[0];
  }
}
```
