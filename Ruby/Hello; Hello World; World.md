## Hello; Hello World; World

Write a function that takes an integer and:
```ruby
If the number is a multiple of 3, return "Hello".
If the number is a multiple of 5, return "World".
If the number is a multiple of both 3 and 5, return "Hello World".

Examples:
hello_world(3) ➞ "Hello"

hello_world(5) ➞ "World"

hello_world(15) ➞ "Hello World"
```
### :gem: My Code
```ruby
def hello_world(n)
 n % 15 == 0 ? 'Hello World' : n % 5 == 0 ? 'World' : 'Hello'
end
```
