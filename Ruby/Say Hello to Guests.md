## Say Hello to Guests
In this exercise you will have to:

Take a list of names.
Add "Hello" to every name.
Make one big string with all greetings.
The solution should be one string with a comma in between every "Hello (Name)".
```ruby
Examples
greet_people(["Joe"]) ➞ "Hello Joe"

greet_people(["Angela", "Joe"]) ➞ "Hello Angela, Hello Joe"

greet_people(["Frank", "Angela", "Joe"]) ➞ "Hello Frank, Hello Angela, Hello Joe"
```
### :gem: My Code
```ruby
def greet_people(names)
  names.map{|x| "Hello " + x}.join(', ')
end
```
