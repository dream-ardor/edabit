## Return the Index of the First Vowel
Create a function that returns the index of the first vowel in a string.
```ruby
Examples
first_vowel("apple") ➞ 0

first_vowel("hello") ➞ 1

first_vowel("STRAWBERRY") ➞ 3

first_vowel("pInEaPPLe") ➞ 1
```
### :gem: My Code
```ruby
def first_vowel(s)
  s.index(/[aeiou]/i)
end
```
