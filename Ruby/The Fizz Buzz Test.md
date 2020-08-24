## The Fizz Buzz Test

The Fizz Buzz test is a poplular interview question used to help filter out the 99.5% of programming job candidates who can't seem to program their way out of a wet paper bag.

Write a program that returns a list of all the numbers from 1 to an integer argument. But for multiples of three use “Fizz” instead of the number and for the multiples of five use “Buzz”. For numbers which are multiples of both three and five use “FizzBuzz”.
```ruby
Example
fizz_buzz(10) ➞ [1, 2, "Fizz", 4, "Buzz", "Fizz", 7, 8, "Fizz", "Buzz"]

fizz_buzz(15) ➞ [1, 2, "Fizz", 4, "Buzz", "Fizz", 7, 8, "Fizz", "Buzz", 11, "Fizz", 13, 14, "FizzBuzz"]
```
### :gem: My Code
```ruby
def fizz_buzz(m)
  (1..m).map{|a|a % 15 == 0 ? 'FizzBuzz' : a % 5 == 0 ? 'Buzz' : a % 3 == 0 ? 'Fizz' : a}
end

```
