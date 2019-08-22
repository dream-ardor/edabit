## Find Unique Positive Numbers from Array
Write a function that takes an array and returns a new array with unique positive (more than 0) numbers.
```ruby
Examples
unique_arr([-5, 1, -7, -5, -2, 3, 3, -5, -1, -1]) ➞ [1, 3]

unique_arr([3, -3, -3, 5, 5, -6, -2, -4, -1, 3]) ➞ [3, 5]

unique_arr([10, 6, -12, 13, 5, 5, 13, 6, 5]) ➞ [10, 6, 13, 5]
```
### :gem: My Code
```ruby
def unique_arr(a)
  a.select{|x| x > 0}.uniq
end
```
## Add, Subtract, Multiply or Divide?
Write a function that takes two numbers and returns if they should be added, subtracted, multiplied or divided to get 24. If none of the operations can give 24, return nil.
```ruby
Examples
operation(15, 9) ➞ "added"

operation(26, 2) ➞ "subtracted"

operation(11, 11) ➞ nil
```
### :gem: My Code
```ruby
def operation(n1, n2)
  n1+n2 == 24 ? "added" : n1-n2 == 24 ? "subtracted"
  : n1*n2 == 24 ? "multiplied" : n1/n2 == 24 ? "divided" : nil
end
```
## Moving to the End
Write a function that moves all elements of one type to the end of the array.
```ruby
Examples
move_to_end([1, 3, 2, 4, 4, 1], 1) ➞ [3, 2, 4, 4, 1, 1]
# Move all the 1s to the end of the array.

move_to_end([7, 8, 9, 1, 2, 3, 4], 9) ➞ [7, 8, 1, 2, 3, 4, 9]

move_to_end(["a", "a", "a", "b"], "a") ➞ ["b", "a", "a", "a"]
```
### :gem: My Code
```ruby
def move_to_end(a, e)
  a.sort_by{|x| x == e ? 1 : 0}
end
```

## Join Two Portions of a Path
Write a function that receives two portions of a path and joins them. The portions will be joined with the "/" separator. There could be only one separator and if it is not present it should be added.
```ruby
Examples
join_path("portion1", "portion2") ➞ "portion1/portion2"

join_path("portion1/", "portion2") ➞ "portion1/portion2"

join_path("portion1", "/portion2") ➞ "portion1/portion2"

join_path("portion1/", "/portion2") ➞ "portion1/portion2"
```
### :gem: My Code
```ruby
def join_path(p1, p2)
  p1.gsub(/\//,'')+ "/" + p2.gsub(/\//,'')
end
```

## Basic Statistics: Mean
The mean of a group of numbers is calculated by summing all numbers, and dividing this sum by the total count of numbers in the group. Given a sorted array of numbers, return the mean (rounded to one decimal place).
```ruby
Examples
mean([1, 6, 6, 7, 8, 8, 9, 10, 10]) ➞ 7.2

mean([1, 3, 8, 9, 9, 10]) ➞ 6.7

mean([2, 3, 3, 6, 6, 8, 9, 10]) ➞ 5.9
```
### :gem: My Code
```ruby
def mean(n)
  (n.reduce(:+).to_f / n.size).round(1)
end
```



