## Buggy Uppercase Counting

In the Code tab is a function which is meant to return how many uppercase letters there are in an array of various words. Fix the code so that it functions normally!
```ruby
Examples
count_uppercase(["SOLO", "hello", "Tea", "wHat"]) ➞ 6

count_uppercase(["little", "lower", "down"]) ➞ 0

count_uppercase(["EDAbit", "Educate", "Coding"]) ➞ 5
```
### :gem: My Code
```ruby
def count_uppercase(a)
  a.map{|x|x.scan(/[A-Z]/)}.join('').size
end 
```
