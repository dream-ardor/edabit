## Recreating a .length Function

Create a function which returns the length of a string, without using .length.
```ruby
Examples
length("Hello World") ➞ 11

length("Edabit") ➞ 6

length("wash your hands!") ➞ 16
```
### :gem: My Code
```ruby
def length(s)
  s == "" ? 0 : s.index(s[-1],-1) + 1
end
```
