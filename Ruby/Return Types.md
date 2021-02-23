## Return Types

Create a function that takes a list lst and returns the types of values (data types) in a new list.
```ruby
Examples
list_values_types([1, 10]), ➞  [Fixnum, Fixnum]

list_values_types([["hello" , 1]  , 10]), ➞  [Array, Fixnum]

list_values_types(["shashwat", 10, 90]), ➞  [String, Fixnum, Fixnum]
```
### :gem: My Code
```ruby
def list_values_types(a)
  a.map(&:class)
end
```
