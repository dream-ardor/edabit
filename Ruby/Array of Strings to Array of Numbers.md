## Array of Strings to Array of Numbers

Create a function that takes as a parameter an array of "stringified" numbers and returns an array of numbers.
```ruby
Example:

["1", "3", "3.6"] ➞ [1, 3, 3.6]
Examples

to_number_array(["9.4", "4.2"]) ➞ [9.4, 4.2]

to_number_array(["21", "23"]) ➞ [21, 23]

to_number_array(["9.5", "8.8"]) ➞ [9.5, 8.8]
```
### :gem: My Code
```ruby
def to_number_array(a)
  a.map(&:to_f)
end
```
