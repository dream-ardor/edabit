## Stupid Addition

Create a function that takes two parameters and, if both parameters are strings, add them as if they were integers or if the two parameters are integers, concatenate them.
```ruby 
Examples
stupid_addition(1, 2) ➞ "12"

stupid_addition("1", "2") ➞ 3

stupid_addition("1", 2) ➞ nil

Notes
If the two parameters are different data types, return nil.
All parameters will either be strings or integers.
```
### 💎 My Code
```ruby
def stupid_addition(a,b)
  a.is_a?(Integer) && b.is_a?(Integer) ? a.to_s + b.to_s :
  a.is_a?(String) && b.is_a?(String) ? a.to_i + b.to_i : nil
end
```
