## Return the Factorial
Create a function that takes an integer and returns the factorial of that integer. That is, the integer multiplied by all positive lower integers.
```ruby
Examples
factorial(3) ➞ 6

factorial(5) ➞ 120

factorial(13) ➞ 6227020800
```
### :mahjong: My Code
```ruby
def factorial(i)
  (1..i).reduce(1,:*)
end
```

## Check if Number is within a Given Range
Given a number and an object with min and max properties, return true if the number lies within the given range (inclusive).
```ruby
Examples
is_in_range(4, { min: 0, max: 5 }) ➞ true

is_in_range(4, { min: 4, max: 5 }) ➞ true

is_in_range(4, { min: 6, max: 10 }) ➞ false

is_in_range(5, { min: 5, max: 5 }) ➞ true
```
### :mahjong: My Code
```ruby
def is_in_range(n, r)
  n.between? *r.values
end
```
## Odd Up, Even Down
Create a function that goes through the array, incrementing (+1) for each odd number and decrementing (-1) for each even number.
```ruby
Examples
transform([1, 2, 3, 4, 5]) ➞ [2, 1, 4, 3, 6]

transform([3, 3, 4, 3]) ➞ [4, 4, 3, 4]

transform([2, 2, 0, 8, 10]) ➞ [1, 1, -1, 7, 9]
```
### :mahjong: My Code
```ruby
def transform(a)
  a.map{|x|x.odd? ? x+1 : x-1}
end
```

## The 3 Programmers Problem
You hired three programmers and you (hopefully) pay them. Create a function that takes three numbers (the hourly wage of each programmer) and returns the difference between the highest-paid programmer and the lowest-paid.
```ruby
Examples
programmers(147, 33, 526) ➞ 493

programmers(33, 72, 74) ➞ 41

programmers(1, 5, 9) ➞ 8
```
### :mahjong: My Code
```ruby
def programmers(*pay)
  pay.max - pay.min
end
```

## Omnipresent Value
A value is omnipresent if it exists in every subarray inside the main array.

To illustrate:

[[3, 4], [8, 3, 2], [3], [9, 3], [5, 3], [4, 3]]
# 3 exists in every element inside this array, so is omnipresent.
Create a function that determines whether an input value is omnipresent for a given array.
```ruby
Examples
is_omnipresent([[1, 1], [1, 3], [5, 1], [6, 1]], 1) ➞ true

is_omnipresent([[1, 1], [1, 3], [5, 1], [6, 1]], 6) ➞ false

is_omnipresent([[5], [5], [5], [6, 5]], 5) ➞ true

is_omnipresent([[5], [5], [5], [6, 5]], 6) ➞ false
```
### :mahjong: My Code
```ruby
def is_omnipresent(a, v)
  a.all?{|x|x.include?(v)}
end
```

## Days in a Month
Create a function that takes the month and year (as integers) and returns the number of days in that month.
```ruby
Examples
day_amount(2, 2018) ➞ 28

day_amount(3, 2011) ➞ 31

day_amount(4, 654) ➞ 30

day_amount(2, 2020) ➞ 29

day_amount(2, 200) ➞ 28

day_amount(2, 1000) ➞ 29
```
### :mahjong: My Code
```ruby
def day_amount(month, year)
  Date.new(year, month, -1).day
end
```

## Mirror Array
Given an array, transform it into a mirror.
```ruby
Examples
mirror([0, 2, 4, 6]) ➞ [0, 2, 4, 6, 4, 2, 0]

mirror([1, 2, 3, 4, 5]) ➞ [1, 2, 3, 4, 5, 4, 3, 2, 1]

mirror([3, 5, 6, 7, 8]) ➞ [3, 5, 6, 7, 8, 7, 6, 5, 3]
```
### :mahjong: My Code
```ruby
def mirror(a)
  a + a.reverse[1..5]
end
```




