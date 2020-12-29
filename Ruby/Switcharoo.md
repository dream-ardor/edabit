## Switcharoo

Create a function that takes a string and returns a new string with its first and last characters swapped, except under three conditions:

If the length of the string is less than two, return "Incompatible.".
If the argument is not a string, return "Incompatible.".
If the first and last characters are the same, return "Two's a pair.".
```ruby
Examples
flipEndChars("Cat, dog, and mouse.") ➞ ".at, dog, and mouseC"

flipEndChars("ada") ➞ "Two's a pair."

flipEndChars("Ada") ➞ "adA"

flipEndChars("z") ➞ "Incompatible."

flipEndChars([1, 2, 3]) ➞ "Incompatible."

Notes
Tests are case sensitive (e.g. "A" and "a" are not the same character).
```
### :gem: My Code
```ruby
def flip_end_chars(s)
 a,b = s[0],s[-1]
 s.size < 2 ? "Incompatible." :
 s.class != String ? "Incompatible." :
 a == b ? "Two's a pair." :
 "#{b}#{s[1..-2]}#{a}"
end
```
