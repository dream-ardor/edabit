## Leap Year Function ⌚

Write a function that returns true if a year is a leap, otherwise it returns false.

A year is a "leap year" if it lasts 366 days, instead of 365 in a typical year. That extra day is added to the end of the shorter month, dating as February 29.

To eliminate this error, the Gregorian calendar stipulates that a year that is divisible by 100 (for example, 1900) is a leap year only if it is also divisible by 400. This is because they are divisible by 100 but not by 400. This is because they're divisible by 100 and 400.

Look at the examples, if you need help look at the resources panel.
```ruby
Examples
leap_year(1990) ➞ false

leap_year(1924) ➞ true
```
### :calendar: My Code
```ruby
def leap_year(y)
  Date.leap?(y)
end
```
