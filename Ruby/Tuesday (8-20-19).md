## Product of All Odd Integers
Create a function that returns the product of all odd integers in an array.
```ruby
Examples
odd_product([3, 4, 1, 1, 5]) ➞ 15

odd_product([5, 5, 8, 2, 4, 32]) ➞ 25

odd_product([1, 2, 1, 2, 1, 2, 1, 2]) ➞ 1
```
### :traffic_light: My Code
```ruby
def odd_product(a)
  a.select(&:odd?).reduce(:*)
end
```

## Check Factors
Write a function that returns true if all integers in an array are factors of a number, and false otherwise.
```ruby
Examples
check_factors([2, 3, 4], 12) ➞ true
# Since 2, 3, and 4 are all factors of 12.

check_factors([1, 2, 3, 8], 12) ➞ false
# 8 is not a factor of 12.

check_factors([1, 2, 50], 100) ➞ true

check_factors([3, 6], 9) ➞ false
```
### :traffic_light: My Code
```ruby
def check_factors(f, n)
  f.all?{|x| n % x == 0}
end
```

## State Names and Abbreviations
Create a function that filters out an array of state names into two categories based on the second parameter.

Abbreviations abb
Full names full
```ruby
Examples
filter_state_names(["Arizona", "CA", "NY", "Nevada"], "abb")
➞ ["CA", "NY"]

filter_state_names(["Arizona", "CA", "NY", "Nevada"], "full")
➞ ["Arizona", "Nevada"]

filter_state_names(["MT", "NJ", "TX", "ID", "IL"], "abb")
➞ ["MT", "NJ", "TX", "ID", "IL"]

filter_state_names(["MT", "NJ", "TX", "ID", "IL"], "full")
➞ []
```

### :traffic_light: My Code
```ruby
def filter_state_names(a, t)
  t == 'abb' ? a.select{|x|x.length == 2} : a.select{|x|x.length > 2}
end
```

## Sort a String by Its Last Character
Create a function that takes a string of words and return a string sorted alphabetically by the last character of each word.
```ruby
Examples
sort_by_last("herb camera dynamic") ➞ "camera herb dynamic"

sort_by_last("stab traction artist approach") ➞ "stab approach traction artist"

sort_by_last("sample partner autonomy swallow trend") ➞ "trend sample partner swallow autonomy"
```
### :traffic_light: My Code
```ruby
def sort_by_last(s)
  s.split(' ').sort_by{|x|x[-1]}.join(' ')
end
```

## Secret Society
A group of friends have decided to start a secret society. The name will be the first letter of each of their names, sorted in alphabetical order.

Create a function that takes in an array of names and returns the name of the secret society.
```ruby
Examples
society_name(["Adam", "Sarah", "Malcolm"]) ➞ "AMS"

society_name(["Harry", "Newt", "Luna", "Cho"]) ➞ "CHLN"

society_name(["Phoebe", "Chandler", "Rachel", "Ross", "Monica", "Joey"]) ➞ "CJMPRR"
```
### :traffic_light: My Code
```ruby
def society_name(f)
  f.map{|x|x[0]}.sort.join
end
```
## Return the Sum of the Two Smallest Numbers
Create a function that takes an array of numbers and returns the sum of the two lowest positive numbers.
```ruby
Examples
sum_two_smallest_nums([19, 5, 42, 2, 77]) ➞ 7

sum_two_smallest_nums([10, 343445353, 3453445, 3453545353453]) ➞ 3453455

sum_two_smallest_nums([2, 9, 6, -1]) ➞ 8

sum_two_smallest_nums([879, 953, 694, -847, 342, 221, -91, -723, 791, -587]) ➞ 563

sum_two_smallest_nums([3683, 2902, 3951, -475, 1617, -2385]) ➞ 4519
```
### :traffic_light: My Code
```ruby
def sum_two_smallest_nums(a)
  b = a.select{|x|x > 0}.sort
  b[0]+b[1]
end
```
## Letters Only
Write a function that removes any non-letters from a string, returning a well-known film title.
```ruby
Examples
letters_only("R!=:~0o0./c&}9k`60=y") ➞ "Rocky"

letters_only("^,]%4B|@56a![0{2m>b1&4i4") ➞ "Bambi"

letters_only("^U)6$22>8p).") ➞ "Up"
```
### :traffic_light: My Code
```ruby
def letters_only(s)
  s.tr('^A-Za-z','')
end
```



