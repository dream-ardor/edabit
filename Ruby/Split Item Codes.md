## Split Item Codes

You have an array of item codes with the following format: "[letters][digits]"

Create a function that splits these strings into their alphabetic and numeric parts.
```ruby
Examples
split_code("TEWA8392") ➞ ["TEWA", 8392]

split_code("MMU778") ➞ ["MMU", 778]

split_code("SRPE5532") ➞ ["SSRPE", 5532]
```
### :snowman: My Code
```ruby
def split_code(i)
  i.scan(/\D+/) + i.scan(/\d+/).map(&:to_i)
end
```
