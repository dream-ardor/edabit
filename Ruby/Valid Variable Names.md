## Valid Variable Names

When creating variables, the variable name must always start with a letter and cannot contain spaces, though numbers and underscores are allowed to be contained in it also.

Create a function which returns true if a given variable name is valid, otherwise return false.
```ruby
Examples
variable_valid("result") ➞ true

variable_valid("odd_nums") ➞ true

variable_valid("2TimesN") ➞ false

Notes:
Inputs are given as strings.
Variable names with spaces are not allowed.
Although this question may seem like otherwise, you can't actually assign words with quotes around them as variables.
```
### :gem: My Code
```ruby
def variable_valid(v)
  !!v.match(/^\D\w+$/)
end
```
