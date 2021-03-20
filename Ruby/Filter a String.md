## Filter a String

Mubashir needs your help to count uppercase letters, lowercase letters, numbers and special characters in a given string.

Create a function which takes a string txt and returns a list of numbers with count of uppercase letters, lowercase letters, numbers and special characters.

Examples
```ruby
filter_string("*$(#Mu12bas43hiR%@*!") ➞ [2, 6, 4, 8]
# 2 uppercase letters
# 6 lowercase letters
# 4 numbers
# 8 special characters

filter_string("^^Edabit^^%$#12379") ➞ [1, 5, 5, 7]

filter_string("**Airforce1**") ➞ [1, 7, 1, 4]
```
### :gem: My Code
```ruby
def filter_string(t)
  [t.scan(/[A-Z]/).size, t.scan(/[a-z]/).size, t.scan(/\d/).size, t.scan(/[\W]/i).size]
end
```
