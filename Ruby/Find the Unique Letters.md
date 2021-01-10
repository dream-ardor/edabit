## Find the Unique Letters

Create a function that takes a string and returns the letters that occur only once.
```ruby
Examples
find_letters("monopoly") ➞ ["m", "n", "p", "l", "y"]

find_letters("balloon") ➞ ["b", "a", "n"]

find_letters("analysis") ➞ ["n", "l", "y", "i"]

Notes:
The final array should not include letters that appear more than once in the string.
Return the letters in the sequence they were originally in, do not sort them.
All letters will be in lowercase.
```
### :gem: My Code
```ruby
def find_letters(w)
  w.chars.select{|a|w.count(a) < 2}
end
```
