## Array From a Range of Numbers

Create a function that returns an array of all the integers between two given numbers start and _end.
```ruby
Examples
range_of_num(2, 4) ➞ [3]

range_of_num(5, 9) ➞ [6, 7, 8]

range_of_num(2, 11) ➞ [3, 4, 5, 6, 7, 8, 9, 10]
```
### :gem: My Code
```ruby
def range_of_num(s,e)
  [*s + 1 .. e - 1]
end
```
