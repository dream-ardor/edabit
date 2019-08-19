## Mirror Array
Given an array, transform it into a mirror.
```
Examples
mirror([0, 2, 4, 6]) ➞ [0, 2, 4, 6, 4, 2, 0]

mirror([1, 2, 3, 4, 5]) ➞ [1, 2, 3, 4, 5, 4, 3, 2, 1]

mirror([3, 5, 6, 7, 8]) ➞ [3, 5, 6, 7, 8, 7, 6, 5, 3]
```
### :stars: My Code
```ruby
def mirror(a)
  a + a.reverse[1..5]
end
```

## Numbers to Arrays and Vice Versa
Write two functions:

to_array(), which converts a number to an array of its digits.
to_number(), which converts an array of digits back to its number.
```ruby
Examples
to_array(235) ➞ [2, 3, 5]

to_array(0) ➞ [0]

to_number([2, 3, 5]) ➞ 235

to_number([0]) ➞ 0
```
### :stars: My Code
```ruby
def to_array(n)
  n.to_s.chars.map(&:to_i)
end

def to_number(a)
  a.join.to_i
end
```
## Repeating Letters N Times
Create a function that repeats each character in a string n times.
```ruby
Examples
repeat("mice", 5) ➞ "mmmmmiiiiiccccceeeee"

repeat("hello", 3) ➞ "hhheeellllllooo"

repeat("stop", 1) ➞ "stop"
```
### :stars: My Code
```ruby
def repeat(s, n)
  s.chars.map{|x|x*n}.join
end
```

## Recursion: Factorials
Write a function that calculates the factorial of a number recursively.
```ruby
Examples
factorial(5) ➞ 120

factorial(3) ➞ 6

factorial(1) ➞ 1

factorial(0) ➞ 1
```
### :stars: My Code
```ruby
def factorial(n)
  n < 2 ? 1 : n * factorial(n-1)
end
```

## Pi to N Decimal Places
Given a number n, write a function that returns PI to n decimal places.
```ruby
Examples
my_pi(5) ➞ 3.14159

my_pi(4) ➞ 3.1416

my_pi(15) ➞ 3.141592653589793
```
### :stars: My Code
```ruby
def my_pi(n)
  Math::PI.round(n)
end
#longer way
def my_pi(n)
  Math.atan2(-0.0, -1.0).round(n) * -1
end
```
## Generate a Countdown of Numbers in an Array
Create a function that takes a number as an argument and returns an array of numbers counting down from this number to zero.
```ruby
Examples
countdown(5) ➞ [5, 4, 3, 2, 1, 0]

countdown(1) ➞ [1, 0]

countdown(0) ➞ [0]
```

### :stars: My Code
```ruby
def countdown(s)
  (0..s).to_a.reverse
end
```

