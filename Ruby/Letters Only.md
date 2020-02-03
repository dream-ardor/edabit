## Letters Only

Write a function that removes any non-letters from a string, returning a well-known film title.
```ruby
Examples
letters_only("R!=:~0o0./c&}9k`60=y") ➞ "Rocky"

letters_only("^,]%4B|@56a![0{2m>b1&4i4") ➞ "Bambi"

letters_only("^U)6$22>8p).") ➞ "Up"
```
### :gem: My Code
```ruby
def letters_only(s)
 s.tr('^A-Za-z', '')
end
```
