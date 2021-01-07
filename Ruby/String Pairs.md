## String Pairs

Create a function that takes a string str and returns an array of two-paired characters. If the string has an odd number of characters, add an asterisk * in the final pair.

See the below examples for a better understanding:
```ruby
Examples
string_pairs("mubashir") ➞ ["mu", "ba", "sh", "ir"]

string_pairs("edabit") ➞ ["ed", "ab", "it"]

string_pairs("airforces") ➞ ["ai", "rf", "or", "ce", "s*"]
```
### :gem: My Code
```ruby
def string_pairs(s)
  "#{s}*".scan(/../)
end
```
