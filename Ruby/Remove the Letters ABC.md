## Remove the Letters ABC

Create a function that will remove the letters "a", "b" and "c" from the given string and return the modified version. If the given string does not contain "a", "b", or "c", return nil.
```ruby
Examples
remove_abc("This might be a bit hard") ➞ "This might e  it hrd"

remove_abc("hello world!") ➞ nil

remove_abc("") ➞ nil

Notes:
If the given string does not contain "a", "b", or "c", return nil.
```
### :gem: My Code
```ruby
def remove_abc(s)
  s.count('abc') > 0  ? s.delete('abc') : nil
end


#alternate solutions
def remove_abc(str)
  str.tr!('abc', '')
end

def remove_abc(str)
  res = str.delete "abc"
  res == str ? nil : res
end
```
