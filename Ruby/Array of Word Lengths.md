## Array of Word Lengths

Create a function that takes an array of words and transforms it into an array of each word's length.
```ruby
Examples
word_lengths(["hello", "world"]) ➞ [5, 5]

word_lengths(["Halloween", "Thanksgiving", "Christmas"]) ➞ [9, 12, 9]

word_lengths(["She", "sells", "seashells", "down", "by", "the", "seashore"]) ➞ [3, 5, 9, 4, 2, 3, 8]
```
### :gem: My Code
```ruby
def word_lengths(a)
  a.map{|a|a.split('').size}
end
```
