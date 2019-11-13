## Array of Consecutive Numbers

Implement a function that returns an array containing all the consecutive numbers in ascendant order from the given value low up to the given value high (bounds included).
```ruby
Examples
get_sequence(1, 5) ➞ [1, 2, 3, 4, 5]

get_sequence(98, 100) ➞ [98, 99, 100]

get_sequence(1000, 1000) ➞ [1000]
```
### :gem: My Code
```ruby
def get_sequence(l,h)
  a = *(l..h)
end
```
