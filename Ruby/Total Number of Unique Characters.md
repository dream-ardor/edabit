## Total Number of Unique Characters
Given two strings, create a function that returns the total number of unique characters from the combined string.
```ruby
Examples
count_unique("apple", "play") ➞ 5
# "appleplay" has 5 unique characters:
# "a", "e", "l", "p", "y"

count_unique("sore", "zebra") ➞ 7

count_unique("a", "soup") ➞ 5
```
### :part_alternation_mark:My Code
```ruby
def count_unique(s1, s2)
  s3 = s1.chars + s2.chars
	s3.uniq.length
end
```
