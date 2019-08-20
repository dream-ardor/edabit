## Moving to the End
Write a function that moves all elements of one type to the end of the array.
```ruby
Examples
move_to_end([1, 3, 2, 4, 4, 1], 1) ➞ [3, 2, 4, 4, 1, 1]
# Move all the 1s to the end of the array.

move_to_end([7, 8, 9, 1, 2, 3, 4], 9) ➞ [7, 8, 1, 2, 3, 4, 9]

move_to_end(["a", "a", "a", "b"], "a") ➞ ["b", "a", "a", "a"]
```
### :sunrise_over_mountains: My Code
```ruby
def move_to_end(a, el)
  a.sort_by{|x| x == el ? 1 : 0}
end
```
## Convert Number to String of Dashes
Create a function that takes a number (from 1 - 60) and returns a corresponding string of hyphens.
```ruby
Examples
num_to_dashes(1) ➞ "-"

num_to_dashes(5) ➞ "-----"

num_to_dashes(3) ➞ "---"
```
### :sunrise_over_mountains: My Code
```ruby
def num_to_dashes(n)
  n = "-" * n
end
```

## Count Ones in a 2D Array
Create a function to count the number of 1s in a 2D array.
```ruby
Examples
count_ones([
  [1, 0],
  [0, 0]
]) ➞ 1

count_ones([
  [1, 1, 1],
  [0, 0, 1],
  [1, 1, 1]
]) ➞ 7

count_ones([
  [1, 2, 3],
  [0, 2, 1],
  [5, 7, 33]
]) ➞ 2
```
### :sunrise_over_mountains: My Code
```ruby
def count_ones(m)
  m.map{|a| a.count(1)}.reduce(:+)
end

#alternatively using flatten
def count_ones(matrix)
  matrix.flatten.count 1
end
```

## Filter out Strings from an Array
Create a function that takes an array of non-negative numbers and strings and return a new array without the strings.
```ruby
Examples
filter_list([1, 2, "a", "b"]) ➞ [1, 2]

filter_list([1, "a", "b", 0, 15]) ➞ [1, 0, 15]

filter_list([1, 2, "aasf", "1", "123", 123]) ➞ [1, 2, 123]
```
### :sunrise_over_mountains: My Code
```ruby
def filter_list(a)
  a.select{|b| b.is_a? Integer}
end
```

## Calculate the Mean
Create a function that takes an array of numbers and returns the mean value.
```ruby
Examples
mean([1, 0, 4, 5, 2, 4, 1, 2, 3, 3, 3]) ➞ 2.54

mean([2, 3, 2, 3]) ➞ 2.50

mean([3, 3, 3, 3, 3]) ➞ 3.00
```
### :sunrise_over_mountains: My Code
```ruby
def mean(a)
  (a.reduce(:+).to_f / a.size).round(2)
end
```

## Largest Swap
Write a function that takes a two-digit number and determines if it's the largest of two possible digit swaps.
```ruby
To illustrate:

largest_swap(27) ➞ false

largest_swap(43) ➞ true
If 27 is our input, we should return false because swapping the digits gives us 72, and 72 > 27. On the other hand, swapping 43 gives us 34, and 43 > 34.

Examples
largest_swap(14) ➞ false

largest_swap(53) ➞ true

largest_swap(99) ➞ true
```
### :sunrise_over_mountains: My Code
```ruby
def largest_swap(n)
  n.to_s.reverse.to_i <= n
end
```

## Flip the Boolean
Create a function that reverses a boolean value and returns the string "boolean expected" if another variable type is given.
```ruby
Examples
reverse(true) ➞ false

reverse(false) ➞ true

reverse(0) ➞ "boolean expected"

reverse(nil) ➞ "boolean expected"
```
### :sunrise_over_mountains: My Code
```ruby
def reverse(b)
  b == true || b == false ? b ^= true : "boolean expected"
end
```

## Convert to Decimal Notation
Create a function to convert an array of percentages to their decimal equivalents.
```ruby
Examples
convert_to_decimal(["1%", "2%", "3%"]) ➞ [0.01, 0.02, 0.03]

convert_to_decimal(["45%", "32%", "97%", "33%"]) ➞ [0.45, 0.32, 0.97, 0.33]

convert_to_decimal(["33%", "98.1%", "56.44%", "100%"]) ➞ [0.33, 0.981, 0.5644, 1]
```
### :sunrise_over_mountains: My Code
```ruby
def convert_to_decimal(p)
  p.map{|x| x.to_f/100 }
end
```

