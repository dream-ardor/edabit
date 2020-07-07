## What's Hiding Amongst the Crowd?

A word is on the loose and now has tried to hide amongst a crowd of tall letters! Help write a function to detect what the word is, knowing the following rules:

The wanted word is in lowercase.
The crowd of letters is all in uppercase.
Note that the word will be spread out amongst the random letters, but their letters remain in the same order.
```ruby
Examples
detect_word("UcUNFYGaFYFYGtNUH") ➞ "cat"

detect_word("bEEFGBuFBRrHgUHlNFYaYr") ➞ "burglar"

detect_word("YFemHUFBbezFBYzFBYLleGBYEFGBMENTment") ➞ "embezzlement"
```
### :gem: My Code
```ruby
def detect_word(t)
  t.chars.select{|a|a==a.downcase}.join
end

#alternate
def detect_word(txt)
  txt.delete "A-Z"
end
```
