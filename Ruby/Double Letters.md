## Double Letters

Create a function that takes a word and returns true if the word has two consecutive identical letters.
```ruby
Examples
double_letters("loop") ➞ true

double_letters("yummy") ➞ true

double_letters("orange") ➞ false

double_letters("munchkin") ➞ false
```
### :gem: My Code
```ruby
def double_letters(w)
  (w=~ /(.)\1+/) != nil
end


#alternate
def double_letters(w)
  w.squeeze != w
end
```
