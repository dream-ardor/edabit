## Verbed Nouns

Create a function that ends the first word of a phrase with "ed", essentially verbifying a noun.
```ruby
Examples
verbify("cheese burger") ➞ "cheesed burger"

verbify("salt water") ➞ "salted water"

verbify("orange juice") ➞ "oranged juice"

verbify("shredded cheese") ➞ "shredded cheese"
```
### :computer: My Code
```ruby
def verbify(s)
  a = s.split[0]
  b = s.split.last
  a.end_with?('e') ? "#{a}d #{b}" : a.end_with?('ed') ? "#{a} #{b}" : "#{a}ed #{b}"
end

#alternate
def verbify(str)
  str.sub(/^(.*?)(ed?)? /, '\1ed ')
end
```
