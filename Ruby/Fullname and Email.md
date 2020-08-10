## Fullname and Email

Create the instance methods fullname and email in the Employee class. Given a person's first and last names:

Form the fullname by simply joining the first and last name together, separated by a space.
Form the email by joining the first and last name together with a . in between, and follow it with @company.com at the end. Make sure everything is in lowercase.
```ruby
Examples
emp_1 = Employee.new("John", "Smith")
emp_2 = Employee.new("Mary",  "Sue")
emp_3 = Employee.new("Antony", "Walker")
emp_1.fullname ➞ "John Smith"

emp_2.email ➞ "mary.sue@company.com"

emp_3.firstname ➞ "Antony"
```
### :gem: My Code
```ruby
class Employee
  attr_reader :firstname, :lastname, :fullname, :email
	
  def initialize(firstname, lastname)
   @firstname = firstname
   @lastname = lastname
  end

  def fullname
    "#{firstname} #{lastname}"
  end

  def email
    "#{firstname}.#{lastname}@company.com".downcase
  end
end
```
