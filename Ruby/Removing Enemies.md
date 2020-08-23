## Removing Enemies

Remove enemies from the array of people, even if the enemy shows up twice.
```ruby
Examples
remove_enemies(["Fred"], []) ➞ ["Fred"]

remove_enemies(["Adam", "Emmy", "Tanya", "Emmy"], ["Emmy"]) ➞ ["Adam", "Tanya"]

remove_enemies(["John", "Emily", "Steve", "Sam"], ["Sam", "John"]) ➞ ["Emily", "Steve"]
```
### :gem: My Code
```ruby
def remove_enemies(n,e)
  n.select{|x|!e.include?(x)}
end
```
