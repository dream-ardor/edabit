## Say "Hello" Say "Bye"

Write a function that takes a string name and a number num (either 0 or 1) and return "Hello" + name if num is 1, otherwise return "Bye" + name.
```ruby
Examples
say_hello_bye("alon", 1) ➞ "Hello Alon"

say_hello_bye("Tomi", 0) ➞ "Bye Tomi"

say_hello_bye("jose", 0) ➞ "Bye Jose"

Notes: 
The name you return must be capitalized.
```
### :gem: My Code
```ruby
def say_hello_bye(a, b)
  b == 1 ? 'Hello ' + a.capitalize : 'Bye ' + a.capitalize
end
```
