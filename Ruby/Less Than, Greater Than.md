## Less Than, Greater Than

Create a function that takes two numbers num1, num2, and an array arr and returns an array containing all the numbers in arr greater than num1 and less than num2.
```ruby
Examples
arr_between(3, 8, [1, 5, 95, 0, 4, 7]) ➞ [5, 4, 7]

arr_between(1, 10, [1, 10, 25, 8, 11, 6]) ➞ [8, 6]

arr_between(7, 32, [1, 2, 3, 78]) ➞ []
```
### :gem: My Code
```ruby
def arr_between(a, b, arr)
  arr.select{|c|c > a && c < b}
end
```
