## Simple OOP Calculator

Create methods for the Calculator class that can do the following:
```
Add two numbers.
Subtract two numbers.
Multiply two numbers.
Divide two numbers.
```
```ruby
Examples
calculator = Calculator.new

calculator.add(10, 5) ➞ 15

calculator.subtract(10, 5) ➞ 5

calculator.multiply(10, 5) ➞ 50

calculator.divide(10, 5) ➞ 2
```
### :gem: My Code
```ruby
class Calculator
def add(a,b)
 a+b
  end
def subtract(a,b)
 a-b
  end
def multiply(a,b)
 a*b
 end
def divide(a,b)
 a/b
 end
end
```
