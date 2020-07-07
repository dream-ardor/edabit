## True Ones, False Zeros

Create a function which returns an array of booleans, from a given number. Iterating through the number one digit at a time, append true if the digit is 1 and false if it is 0.
```ruby
Examples
integer_boolean("100101") ➞ [true, false, false, true, false, true]

integer_boolean("10") ➞ [true, false]

integer_boolean("001") ➞ [false, false, true]
```
### :gem: My Code
```ruby
def integer_boolean(n)
  n.chars.map{|a|a == '1'}
end
```
