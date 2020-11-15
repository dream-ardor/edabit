## Converting Hashes to Arrays

Write a function that converts a hash into an array, where each element represents a key-value pair in the form of an array.
```ruby
Examples
convert_to_array({ "a" => 1, "b" => 2 }) ➞ [["a", 1], ["b", 2]]

convert_to_array({ "shrimp" => 15, "tots" => 12 }) ➞ [["shrimp", 15], ["tots", 12]]

convert_to_array({}) ➞ []
```
### :gem: My Code
```ruby
def convert_to_array(h)
  [*h]
end
```
